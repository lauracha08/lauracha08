<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mapa Institución Educativa Virgen del Carmen</title>
    <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY"></script>
    <style>
        /* Estilo para el mapa */
        #map {
            height: 100vh; /* Altura del mapa */
            width: 100%; /* Ancho del mapa */
        }
    </style>
</head>
<body>
    <h1>Mapa de la Institución Educativa Virgen del Carmen</h1>
    <div id="map"></div>
    <script>
        function initMap() {
            // Coordenadas de la Institución Educativa Virgen del Carmen
            const location = { lat: 10.46314, lng: -73.25153 };

            // Crear el mapa centrado en la ubicación
            const map = new google.maps.Map(document.getElementById("map"), {
                zoom: 15, // Nivel de zoom
                center: location, // Centro del mapa
            });

            // Añadir un marcador en la ubicación
            new google.maps.Marker({
                position: location,
                map: map,
                title: "Institución Educativa Virgen del Carmen",
            });
        }

        // Inicializar el mapa al cargar la página
        window.onload = initMap;
    </script>
</body>
</html>
