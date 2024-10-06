# world-map.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Environmental Data Map</title>
    <link rel="stylesheet" href="style.css"> <!-- Fixed the href attribute -->
    <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
    <style>
        /* Added some basic styles for the header, main, and sidebar */
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 20px;
            text-align: center;
        }
        h1 {
            margin: 0;
            font-size: 2.5em;
        }
        main {
            display: flex;
        }
        #map {
            flex: 1; /* Allows the map to take up available space */
            height: 600px; /* Set a height for the map */
        }
        #sidebar {
            width: 300px; /* Set a fixed width for the sidebar */
            padding: 20px;
            background-color: #f4f4f4;
            border-left: 1px solid #ccc;
        }
        h2 {
            color: #4CAF50; /* Fixed color style */
            margin-bottom: 10px;
        }
        footer {
            text-align: center;
            padding: 10px;
            background-color: #f4f4f4;
            border-top: 1px solid #ccc;
        }
    </style>
</head>
<body>
    <header>
        <h1>EARTHSYNC</h1>
    </header>
    <main>
        <div id="map" aria-label="Map displaying environmental data"></div>
        <aside id="sidebar">
            <h2>City Information</h2>
            <div id="city-info">
                <p>Select a city to see data.</p>
            </div>
        </aside>
    </main>
    <footer>
        <p>&copy; 2024 EARTHSYNC. All rights reserved.</p>
    </footer>
    
    <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
    <script src="script.js"></script>
</body>
</html>
