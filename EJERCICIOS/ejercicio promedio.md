# EJERCICIO

## VERSION 1 

calcular el promeddio de un estudiante de PILARES

primer periodo

taller:6.7

computo; 8.0
    
segundo periodo

taller:5.7

computo; 9
    
tercer periodo

taller:9.92

computo; 6.8
    
calcular y mostrar por consola promedio por periodo y promedio general, ademas del status APROBADO o REPROBADO.

        var taller= parseInt(prompt("Ingresa la calificacion de taller"));
        var computo = parseInt(prompt("Ingresa la calificacion de computo"));;
        var periodo1 = (taller + computo)/2;
        console.log("Periodo 1: "  + periodo1);
        taller= parseInt(prompt("Ingresa la calificacion de taller"));
        computo = parseInt(prompt("Ingresa la calificacion de computo"));
        var periodo2 = (taller + computo)/2;
        console.log("Periodo 2: "  + periodo2);
        taller= parseInt(prompt("Ingresa la calificacion de taller"));
        computo = parseInt(prompt("Ingresa la calificacion de computo"));
        var periodo3 = (taller + computo)/2;
        console.log("Periodo 3: "  + periodo3);
        var promedio = (periodo1 + periodo2 + periodo3) / 3;
        
        console.log("Promedio: "  + promedio);
        
        if(promedio > 6){
            console.log("APROBADO");
        }else{
            console.log("REPROBADO");
        }

## VERSION 2
Se deben solicitar por prompt las calificaciones y además agregar el nombre del estudiante, también su estatus de acuerdo al promedio general, menor de 6 es REPROBADO, de 6.1 a 8 es BIEN, de 8.1 a 9 es MUY BIEN y de 9.1 a 10 es EXCELENTE.

        var captura = confirm("Deseas capturar un alumno ");
        if(captura == true){
            var calificacion = parseFloat(prompt("ingresa la calificación"));
            var suma = 0;
            suma = suma + calificacion;
            calificacion = parseFloat(prompt("ingresa la calificación"));
            suma = suma + calificacion;
            calificacion = parseFloat(prompt("ingresa la calificación"));
            suma = suma + calificacion;
            var periodo1 = suma / 3;
            suma = 0;
            calificacion = parseFloat(prompt("ingresa la calificación"));
            suma = suma + calificacion;
            calificacion = parseFloat(prompt("ingresa la calificación"));
            suma = suma + calificacion;
            calificacion = parseFloat(prompt("ingresa la calificación"));
            suma = suma + calificacion;
            var periodo2 = suma/3;
            suma = 0;
            calificacion = parseFloat(prompt("ingresa la calificación"));
            suma = suma + calificacion;
            calificacion = parseFloat(prompt("ingresa la calificación"));
            suma = suma + calificacion;
            calificacion = parseFloat(prompt("ingresa la calificación"));
            suma = suma + calificacion;
            var periodo3 = suma/3;
            var promedio = (periodo1  + periodo2 + periodo3)/3;
            // alert("periodo 1: "  + periodo1 + "\nperiodo2: " + periodo2);
            alert(`periodo 1: ${periodo1} \nperiodo2: ${periodo2} \nperiodo3: ${periodo3} \npromedio: ${promedio} `);
        
            switch(true){
                case promedio < 6:
                    alert("REPROBADO");
                    break;
                case promedio < 8:
                    alert("BIEN");
                    break;
                case promedio < 10:
                    alert("MUY BIEN");
                    break;
                case promedio == 10:
                    alert("EXCELENTE");
                    break;
            }
        
        }else{
            alert("Adios ");
        }


## VERSION 3
Se deben pedir datos de N número de alumnos y los periodos deben estar en ciclo

    var captura = confirm("Deseas capturar un alumno ");
    
    while(captura == true){
        var sumaPeriodo = 0;
        for(var j = 0;j < 3;j++){
            var suma = 0;
            var promedioPeriodo=0;
            for(var i = 0;i < 3; i++){
                var calificacion = parseFloat(prompt(`ingresa la calificación ${i +1} del periodo ${j+1}`));
                var suma = suma + calificacion;
            }
            promedioPeriodo = suma/3;
            alert(`promedio del periodo  ${j + 1} = ${promedioPeriodo}`);
            sumaPeriodo = sumaPeriodo + promedioPeriodo;
        }
        var promedio = sumaPeriodo/3;
    
        switch(true){
            case promedio < 6:
                alert(`REPROBADO, PROMEDIO: ${promedio}`);
                break;
            case promedio < 8:
                alert(`BIEN, PROMEDIO: ${promedio}`);
                break;
            case promedio < 10:
                alert(`MUY BIEN, PROMEDIO: ${promedio}`);
                break;
            case promedio == 10:
                alert(`EXCELENTE, PROMEDIO: ${promedio}`);
                break;
        }
    
        captura = confirm("Deseas capturar un alumno ");
    }
    alert("Adios ");



## VERSION 4
Se debe agregar la fecha de las calificaciones y poder visualizalas

![image](https://github.com/user-attachments/assets/ef1eb5f4-f3c6-4295-9142-850ec73c6add)

