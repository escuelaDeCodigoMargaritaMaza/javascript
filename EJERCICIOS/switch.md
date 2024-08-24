## VERSON 1 

### HTML
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
        <h1>Switch en JS</h1>
    </body>
    </html>

### JS

    var dia = 2;
    
    switch (dia){
        case 1:
            console.log("es lunes");
            break;
        case 2:
            console.log("es martes");
            break;
        case 3:
            console.log("es miercoles");
            break;
        case 4:
            console.log("es jueves");
            break;
        case 5:
            console.log("es viernes");
            break;
        case 6:
            console.log("es sábado");
            break;
        case 7:
            console.log("es domingo");
            break;
        default:
            console.log("dia invalido");
    }

## VERSION 2

### JS

      var dia = parseInt(prompt("ingresa el dia de la semana"));
    
       switch (dia){
        case 1:
            console.log("es lunes");
            break;
        case 2:
            console.log("es martes");
            break;
        case 3:
            console.log("es miercoles");
            break;
        case 4:
            console.log("es jueves");
            break;
        case 5:
            console.log("es viernes");
            break;
        case 6:
            console.log("es sábado");
            break;
        case 7:
            console.log("es domingo");
            break;
        default:
            console.log("dia invalido");
    }
