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

css.

        body{
            background-color: #f4f4f4;
            font-family: Arial,sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        
        .contenedor{
            background-color: #fff;
            padding: 10px;
            border-radius: 10px;
            box-shadow: 0 0 10px black;
        }
        .convertidor{
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        button{
            background-color: rgb(157, 166, 243);
            color: #fff;
            padding: 5px;
            border: none;
            border-radius: 5px;
        }
        button:hover{
            background-color: rgb(91, 41, 243);
        } 
        #datosSalida{
            font-size: 1.5em;
            color:#333;
        }
                    <button onclick="convertir()">Convertir 🌫</button>
                </div>
                <p id="datosSalida"></p>
            </div>
        
            <script src="js/main.js"></script>
        </body>
        </html>
