<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portal de Accesos Terranova</title>
    <style>
        @font-face {
            font-family: 'PP Fragment Glare Regular';
            src: url('ruta/a/PPFragmentGlareRegular.woff2') format('woff2');
        }
        @font-face {
            font-family: 'PP Fragment Sans Regular';
            src: url('ruta/a/PPFragmentSansRegular.woff2') format('woff2');
        }
        body {
            font-family: 'PP Fragment Sans Regular', sans-serif;
            background: linear-gradient(90deg, #F5F5DC 100%, #264746 100%); /* hueso y Teal
            color: #264746; /* Hueso */
            text-align: center;
           px;
            margin: 0;
        }
        .titulo {
            background-color: #264746; /* Color Teal*/
            color: #F5F5DC; /* Color hueso */
            padding: 40px;
            text-align: center;
            transition: background-color 0.3s, color 0.3s;
            width: 100%;
            position: absolute;
            top: 0;
            left: 0;
            box-sizing: border-box;
        }
        .titulo:hover {
            background-color: #008080; /* Color Teal */
            color: #F5F5DC; /* Color hueso */
        }
        h1 {
            font-family: 'PP Fragment Glare Regular', sans-serif;
            font-size: 3em;
            margin: 50;
        }
        .section {
            margin: 10px;
            padding-top: 100px; /* Para evitar que el contenido quede detrás del título */
        }
        .section h2 {
            font-family: 'PP Fragment Glare Regular', sans-serif;
            font-size: 2em;
            margin-bottom: 20px;
        }
        .button-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 25px;
        }
        .button {
            background: #264746; /* Menta */
            border: none;
            padding: 15px 50px; /* Botones más anchos */
            font-size: 1.2em;
            color: rgb(236, 226, 210); /* Hueso */
            border-radius: 50px; /* Bordes redondeados */
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            position: relative;
            overflow: hidden;
        }
        .button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: rgba(255, 255, 255, 0.2);
            transition: all 0.3s ease;
        }
        .button:hover::before {
            left: 100%;
        }
        .button:hover {
            background: #008080; /* Pino más oscuro */
            box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
        }
        .copy-icon {
            position: absolute;
            top: 7.5px;
            right: 10px;
            background: rgba(255, 255, 255, 0.3);
            border-radius: 50%;
            padding: 4px;
            cursor: pointer;
            display: none;
        }
        .button:hover .copy-icon {
            display: block;
        }
        .copy-icon::before {
            content: '\1F4CB'; /* Icono de portapapeles */
            font-size: 1.2em;
            color: rgb(236, 226, 210); /* Hueso */
        }
    </style>
    <script>
        function copyToClipboard(text) {
            navigator.clipboard.writeText(text).then(function() {
                alert('Enlace copiado al portapapeles');
            }, function(err) {
                console.error('Error al copiar el enlace: ', err);
            });
        }
    </script>
</head>
<body>
    <div class="titulo">
        <h1>Accesos Terranova Costa Rica</h1>
    </div>

    <div class="section">
	<h1>-</h1>
        <h2>Solicitud de Apertura</h2>
        <div class="button-container">
            <button class="button" onclick="location.href='http://perfiles.terranova.co.cr/facturacion/new'">
                Solicitud en Zeus
                <span class="copy-icon" onclick="copyToClipboard('http://perfiles.terranova.co.cr/facturacion/new'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://forms.office.com/pages/responsepage.aspx?id=jN90G6rIeUWdbBRw0MTogTKrGmVsDR1FvMOrqJ5zYbhUQjZUTDgxMDU4MDMyWkpKNU9ZTjhITUgzTC4u'">
                Solicitud en Toursys
                <span class="copy-icon" onclick="copyToClipboard('https://forms.office.com/pages/responsepage.aspx?id=jN90G6rIeUWdbBRw0MTogTKrGmVsDR1FvMOrqJ5zYbhUQjZUTDgxMDU4MDMyWkpKNU9ZTjhITUgzTC4u'); event.stopPropagation();"></span>
            </button>
        </div>
    
        <h2>Sistemas</h2>
        <div class="button-container">
            <button class="button" onclick="location.href='https://k8s-cloud1.toursys.net/Toursys/login.xhtml?companyName=Terranova'">
                Toursys
                <span class="copy-icon" onclick="copyToClipboard('https://k8s-cloud1.toursys.net/Toursys/login.xhtml?companyName=Terranova'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://account.wetu.com/'">
                Wetu
                <span class="copy-icon" onclick="copyToClipboard('https://account.wetu.com/'); event.stopPropagation();"></span>
            </button>
        </div>
 
        <h2>Reservas</h2>
        <div class="button-container">
            <button class="button" onclick="location.href='https://www.hotelreservations.com'">
                Reservas de Hoteles 1
                <span class="copy-icon" onclick="copyToClipboard('https://www.hotelreservations.com'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://www.hotelbookings.com'">
                Reservas de Hoteles 2
                <span class="copy-icon" onclick="copyToClipboard('https://www.hotelbookings.com'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://www.hotelbookingexample.com'">
                Reservas de Hoteles 3
                <span class="copy-icon" onclick="copyToClipboard('https://www.hotelbookingexample.com'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://www.hotelbookingexample2.com'">
                Reservas de Hoteles 4
                <span class="copy-icon" onclick="copyToClipboard('https://www.hotelbookingexample2.com'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://www.hotelbookingexample3.com'">
                Reservas de Hoteles 5
                <span class="copy-icon" onclick="copyToClipboard('https://www.hotelbookingexample3.com'); event.stopPropagation();"></span>
            </button>
        </div>
    
        <h2>Producto</h2>
        <div class="button-container">
            <button class="button" onclick="location.href='https://midestinoseguro.terranova.co.cr/'">
                CMDS
                <span class="copy-icon" onclick="copyToClipboard('https://midestinoseguro.terranova.co.cr/'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://curatedexperiences.terranovacostarica.com/'">
                Tours en Inglés
                <span class="copy-icon" onclick="copyToClipboard('https://curatedexperiences.terranovacostarica.com/'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://experienciasexclusivas.terranovacostarica.com/'">
                Tours en Español
                <span class="copy-icon" onclick="copyToClipboard('https://experienciasexclusivas.terranovacostarica.com/'); event.stopPropagation();"></span>
            </button>
            <button class="button" onclick="location.href='https://terranovacocr.sharepoint.com/:f:/s/repositorio/comercial/EszJXx5NvKJDkRRG33O7ZAMBMOP-ACH1361WJ7JnwT3diA?e=ucYroo'">
		SharedPoint
                <span class="copy-icon" onclick="copyToClipboard('https://terranovacocr.sharepoint.com/:f:/s/repositorio/comercial/EszJXx5NvKJDkRRG33O7ZAMBMOP-ACH1361WJ7JnwT3diA?e=ucYroo'); event.stopPropagation();"></span>
            </button>
        </div>
    </div>
</body>
</html>

