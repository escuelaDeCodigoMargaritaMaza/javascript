EJERCICIO

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

## VERSION 3
Se deben pedir datos de N número de alumnos y los periodos deben estar en ciclo
