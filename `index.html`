<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¡Gracias por visitarnos!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
            padding: 50px;
        }
        h1 {
            color: #333;
        }
        p {
            font-size: 1.2em;
            color: #555;
        }
        .motivacion {
            margin-top: 30px;
            font-style: italic;
            color: #777;
        }
    </style>
    <script>
        // Función para registrar la visita
        function registrarVisita() {
            const url = 'https://tuservidor.com/registrar-visita'; // Cambia esto por la URL de tu servidor
            const datos = {
                ip: '<?php echo $_SERVER['REMOTE_ADDR']; ?>', // Obtiene la IP del visitante
                userAgent: navigator.userAgent, // Obtiene el navegador y sistema operativo
                fecha: new Date().toISOString() // Obtiene la fecha y hora
            };

            fetch(url, {
                method: 'POST',
                headers: {
                    'Content-Type': 'application/json'
                },
                body: JSON.stringify(datos)
            });
        }

        // Llama a la función cuando la página se carga
        window.onload = registrarVisita;
    </script>
</head>
<body>
    <h1>¡Gracias por visitarnos!</h1>
    <p>Esta es una demostración educativa sobre seguridad informática.</p>

    <div class="motivacion">
        <p>💪 ¡Tú puedes lograr todo lo que te propongas!</p>
        <p>🚀 El éxito es la suma de pequeños esfuerzos repetidos día tras día.</p>
        <p>🌟 Cada día es una nueva oportunidad para brillar.</p>
        <p>🔥 No te rindas, los grandes resultados requieren tiempo y dedicación.</p>
        <p>🌈 Después de la tormenta siempre sale el sol.</p>
    </div>
</body>
</html>
