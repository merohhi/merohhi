<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Map Webpage</title>
    <!-- Add any additional CSS styles here -->
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
        }
        #map {
            height: 500px; /* Adjust the height of your map */
            width: 100%; /* Make the map take up the full width of the viewport */
        }
    </style>
</head>
<body>
    <!-- Add your map here -->
    <div id="map"></div>

    <!-- Replace the API key with your own Google Maps API key -->
    <script src="https://maps.googleapis.com/maps/api/js?key=YOUR_API_KEY&callback=initMap" async defer></script>
    <script>
        // Initialize and display the map
        function initMap() {
            // Set the coordinates for the center of your map
            var center = { lat: 40.7128, lng: -74.0060 }; // New York City coordinates as an example

            // Create a new map object and center it on the specified coordinates
            var map = new google.maps.Map(document.getElementById('map'), {
                center: center,
                zoom: 10 // Adjust the initial zoom level as needed
            });

            // You can add markers, polygons, or other map elements here
        }
    </script>
</body>
</html>
