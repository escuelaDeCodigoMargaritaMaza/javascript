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
        <h1>Bucles en JS</h1>
    </body>
    </html>

### JS

    //bucle while
    //convensión iniciar contadores en 0
    
    console.log("Bucle while");
    var contador = 0;
    var veces = parseInt(prompt("ingresa el número de ciclos"));
    
    while(contador < veces){
        console.log("ciclo: " + contador);
        contador ++; // de no aumentar entraremos en un bucle infinito
    }
    
    //bucle for
    console.log("Bucle for");
    for(var i = 1;i < 10;i++){
        console.log("ciclo: " + i);
    }
    
    //bucle do while
    
    console.log("Bucle do while");
    var contador1 = 10;
    
    do{
        console.log("ciclo: " + contador1);
        contador1++;
    }
    while(contador1 < 10)
