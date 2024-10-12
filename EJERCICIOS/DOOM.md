html

      <!DOCTYPE html>
      <html lang="en">
      <head>
          <meta charset="UTF-8">
          <meta name="viewport" content="width=device-width, initial-scale=1.0">
          <title>Ejercicio</title>
          <link rel="stylesheet" href="css/estilos.css">
      
      </head>
      <body>
          <div class="contenedor">
              <h1>contador de visitas</h1>
              <p>Visitas <span id="contador">0</span></p>
              <button>Contar visita</button>
          </div>
          
          <script src="js/index.js">          </script>
      </body>
      </html>

css

      body {
          font-family: Arial, sans-serif;
          background-color: #f4f4f4;
          color: #333;
          margin: 0;
          padding: 20px;
      }
      
      
      .contenedor {
          max-width: 600px;
          margin: 0 auto;
          padding: 20px;
          border: 1px solid #ccc;
          border-radius: 10px;
          background-color: #fff;
          box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
          text-align: center;
      }


      h1 {
          color: #4CAF50;
      }
      
      
      button {
          padding: 10px 20px;
          font-size: 16px;
          color: #fff;
          background-color: #4CAF50;
          border: none;
          border-radius: 5px;
          cursor: pointer;
      }
      
      
      button:hover {
          background-color: #45a049;
      }
