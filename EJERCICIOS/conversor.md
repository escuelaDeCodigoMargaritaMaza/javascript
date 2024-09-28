    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Conversor</title>
        <link rel="stylesheet" href="css/estilos.css">
    </head>
    <body>
        <div class="contenedor">
            <h1>Conversor de unidades</h1>
            <div class="convertidor">
                Cantidad a convertir <input type="number" id="cantidadEntrada">
                Unidad de Entrada.
                <select id="unidadEntrada">
                    <option>selecciona</option>
                    <option value="metros">metros</option>
                    <option value="kilometros">kilometros</option>
                    <option value="gramos">gramos</option>
                    <option value="kilos">kilos</option>
                    <option value="celsius">celsius</option>
                    <option value="fahrengeit">fahrengeit</option>
                </select>
                Unidad de Salida
                <select id="unidadSalida">
                    <option>selecciona</option>
                    <option value="metros">metros</option>
                    <option value="kilometros">kilometros</option>
                    <option value="gramos">gramos</option>
                    <option value="kilos">kilos</option>
                    <option value="celsius">celsius</option>
                    <option value="fahrengeit">fahrengeit</option>
                </select>
            </div>
        </div>
    
        <script src="js/main.js"></script>
    </body>
    </html>
