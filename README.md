# juliettelasso.github.io

<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8">
    <title>Mi ubicación GPS</title>
  </head>
  <body>
    <h1 id="location">Cargando ubicación...</h1>
    <script>
      if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(function(position) {
          var latitude = position.coords.latitude;
          var longitude = position.coords.longitude;
          document.getElementById("location").innerHTML =
            "Latitud: " + latitude + "<br>Longitud: " + longitude;
        });
      } else {
        document.getElementById("location").innerHTML =
          "Lo siento, tu navegador no soporta la ubicación GPS.";
      }
    </script>
  </body>
</html>
![image](https://user-images.githubusercontent.com/57605283/219997799-e4d4f1c5-a472-4105-bb7f-76ab0dd4755e.png)
