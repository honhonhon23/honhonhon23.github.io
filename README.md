 <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
     integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
     crossorigin=""/>

      <!-- Make sure you put this AFTER Leaflet's CSS -->
 <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
     integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
     crossorigin=""></script>

     

# GeoIT Projekte

## Navigation
- [Home](#home)
- [About](#about)
- [Services](#services)
- [Contact](#contact)

---

## Home
Welcome to my clean website! This is a simple template to get you started.
 

### Featured Content
- Latest News: Stay updated with the latest news and articles.
- Upcoming Events: Check out our upcoming events and activities.

---

## About
This section provides information about the website or the organization. You can include your mission, vision, and values here.

### Our Mission
To provide quality content and services to our users.

---

## Services
Here you can list the services you offer.

1. Service One: Description of service one.
2. Service Two: Description of service two.
3. Service Three: Description of service three.

---

## Contact
If you have any questions, feel free to reach out!

- Email: [info@example.com](mailto:info@example.com)
- Phone: (123) 456-7890

<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Karte von Berlin mit Leaflet</title>
    <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
    <style>
        #map {
            height: 600px; / Höhe der Karte /
            width: 100%; / Breite der Karte /
        }
    </style>
</head>
<body>

    <h1>Karte von Berlin</h1>
    <div id="map"></div>

    <script src="" target="_blank">https://unpkg.com/leaflet/dist/leaflet.js"></script>
    <script>
        // Erstelle die Karte und setze den Startpunkt auf Berlin
        var map = L.map('map').setView([52.5200, 13.4050], 13); // Koordinaten für Berlin

        // Füge eine Tile-Layer hinzu (Kartenmaterial)
        L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
            maxZoom: 19,
            attribution: '© OpenStreetMap'
        }).addTo(map);

        // Füge einen Marker für Berlin hinzu
        var marker = L.marker([52.5200, 13.4050]).addTo(map);
        marker.bindPopup("<b>Berlin!</b><br>Hauptstadt von Deutschland.").openPopup();
    </script>

</body>
</html>


---

## Footer
© 2023 My Clean Website. All rights reserved.
