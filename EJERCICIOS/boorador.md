## VERSION 7
Agregar métodos de cadenas

    // Función para pedir el nombre del alumno con validación usando length y toUpperCase
    function pedirNombre() {
        var nombre = "";
        while (!nombre || nombre.length < 3) {  // Validamos que el nombre tenga al menos 3 caracteres
            nombre = prompt("Ingresa el nombre del alumno (mínimo 3 caracteres)");
            if (!nombre || nombre.length < 3) {
                alert("El nombre debe tener al menos 3 caracteres. Inténtalo de nuevo.");
            }
        }
        nombre = nombre.toUpperCase();  // Convertir el nombre a mayúsculas
        return nombre;
    }
    
    // Función para pedir las calificaciones de un alumno
    function pedirCalificaciones() {
        var calificaciones = [];
        for (var i = 0; i < 3; i++) {
            var calificacion = parseFloat(prompt("Ingresa la calificación " + (i + 1)));
            calificaciones.push(calificacion);
        }
        return calificaciones;
    }
    
    // Función para calcular el promedio de las calificaciones
    function calcularPromedio(calificaciones) {
        var suma = 0;
        for (var i = 0; i < calificaciones.length; i++) {
            suma += calificaciones[i];
        }
        var promedio = suma / calificaciones.length;
        return promedio;
    }
    
    // Función principal para capturar datos y mostrar resultados
    function capturarDatos() {
        var nombres = [];
        var promedios = [];
        var captura = confirm("¿Deseas capturar un alumno?");
    
        while (captura) {
            var nombre = pedirNombre();
            if (nombres.includes(nombre)) {
                alert("El nombre '" + nombre + "' ya ha sido agregado. No se puede repetir.");
            } else {
                var calificaciones = pedirCalificaciones();
                var promedio = calcularPromedio(calificaciones);
    
                nombres.push(nombre);
                promedios.push(promedio);
    
                captura = confirm("¿Deseas capturar otro alumno?");
           }
        }
    
        alert("Adiós");
    
        // Mostrar nombres y promedios
        for (var i = 0; i < nombres.length; i++) {
            console.log("Nombre: " + nombres[i] + ", Promedio: " + promedios[i]);
        }
    }
    
    // Llamar a la función principal para iniciar el proceso
    capturarDatos();


## VERSION 8
Plasmar los resultados en DOM

    // Función para pedir el nombre del alumno con validación usando length y toUpperCase
    function pedirNombre() {
        var nombre = "";
        while (!nombre || nombre.length < 3) {  // Validamos que el nombre tenga al menos 3 caracteres
            nombre = prompt("Ingresa el nombre del alumno (mínimo 3 caracteres)");
            if (!nombre || nombre.length < 3) {
                alert("El nombre debe tener al menos 3 caracteres. Inténtalo de nuevo.");
            }
        }
        nombre = nombre.toUpperCase();  // Convertir el nombre a mayúsculas
        return nombre;
    }
    
    // Función para pedir las calificaciones de un alumno
    function pedirCalificaciones() {
        var calificaciones = [];
        for (var i = 0; i < 3; i++) {
            var calificacion = parseFloat(prompt("Ingresa la calificación " + (i + 1)));
            calificaciones.push(calificacion);
        }
        return calificaciones;
    }
    
    // Función para calcular el promedio de las calificaciones
    function calcularPromedio(calificaciones) {
        var suma = 0;
        for (var i = 0; i < calificaciones.length; i++) {
            suma += calificaciones[i];
        }
        var promedio = suma / calificaciones.length;
        return promedio;
    }
    
    // Función principal para capturar datos y mostrar resultados en el DOM
    function capturarDatos() {
        var nombres = [];
        var promedios = [];
        var captura = confirm("¿Deseas capturar un alumno?");
    
        while (captura) {
            var nombre = pedirNombre();
            if (nombres.includes(nombre)) {
                alert("El nombre '" + nombre + "' ya ha sido agregado. No se puede repetir.");
            } else {
                var calificaciones = pedirCalificaciones();
                var promedio = calcularPromedio(calificaciones);
    
                nombres.push(nombre);
                promedios.push(promedio);
    
                mostrarEnDom(nombre, promedio);
    
                captura = confirm("¿Deseas capturar otro alumno?");
            }
        }
    
        alert("Adiós");
    }
    
    // Función para mostrar el nombre y promedio en el DOM
    function mostrarEnDom(nombre, promedio) {
        var listaAlumnos = document.getElementById("lista-alumnos");
        var li =    ("li");
        li.textContent = "Nombre: " + nombre + ", Promedio: " + promedio.toFixed(2);
        listaAlumnos.appendChild(li);
    }
    
    // Escuchar el clic del botón para iniciar la captura
    document.getElementById("capturar-btn").addEventListener("click", function() {
        capturarDatos();
    });
    
    
    // Supongamos que tienes un botón en tu HTML con el ID "miBoton"
    <button id="miBoton">Haz clic aquí</button>
    
    // Puedes añadir un evento de clic a este botón de la siguiente manera:
    var boton = document.getElementById("miBoton");
    
    boton.addEventListener("click", function() {
        alert("¡El botón fue clickeado!");
    });


HTML

    <!DOCTYPE html>
    <html lang="es">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        
        <title>Registro de Alumnos</title>
    </head>
    <body>
        <h1>Captura de Alumnos y Promedios</h1>
    
        <button id="capturar-btn">Capturar Alumno</button>
    
        <h2>Lista de Alumnos</h2>
        <ul id="lista-alumnos">
            <!-- Aquí se agregarán los alumnos -->
        </ul>
    
        <script src="js/main.js"></script>
    </body>
    </html>


CSS

    p{
        font-size: 2em;
        color: blue;
        text-align: center;
    }
