<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Página de Prueba</title>
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
    <h1>¡
