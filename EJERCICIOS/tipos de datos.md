## HTML
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Taller JS</title>
        <link rel="stylesheet" href="css/estilos.css">
        <script src="js/main.js"></script>
    </head>
    <body>
        <h1>Tipos de datos y variables en JS</h1>
    </body>
    </html>
    
## JS

    var nombre="david";
    var apellido="Pérez";
    var inscritoONo=true;
    var edad=45;
    let califPrevia = "7";

    console.log("Nombre: " + nombre );
    console.log("Apellido: " + apellido);
    console.log("Inscrito: " + inscritoONo);
    console.log("Edad: " + edad);
    console.log("calificación previa: " + califPrevia);

## VERSION 2

### JS
    var nombre="david";
    var apellido="Pérez";
    var inscritoONo=true;
    var edad=45;
    let califPrevia = "7";

    console.log("Nombre: " + nombre + " y es de tipo " + typeof nombre);
    console.log("Apellido: " + apellido+ " y es de tipo " + typeof apellido);
    console.log("Inscrito: " + inscritoONo + " y es de tipo " + typeof inscritoONo);
    console.log("Edad: " + edad + " y es de tipo " + typeof edad);
    console.log("calificación previa: " + califPrevia + " y es de tipo " + typeof califPrevia);

## VERSION 3
### JS
    //DIFERENCIA VAR LET
    if(true){
        let peso = 43.5;
        //console.log("peso: " + peso + " y es de tipo " + typeof peso);
    }
    //console.log("peso: " + peso + " y es de tipo " + typeof peso);
