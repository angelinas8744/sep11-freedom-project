# Entry 4
##### 3/18/22
### Overview
This month has been very very sucessful in terms of my freedom project. I was able to sucessfully create a working map with my disried coordanetes, as well as working zoom features. It wasnt as hard as I thought, and I am perfectly in time with my [MVP Plan](https://docs.google.com/document/d/1WPoUtDxDtXmFJ1bUfcMtytF-ZiVZD5GwN2wqt8km6Hc/edit?usp=sharing). The MVP is the Minimum Value Product. As long as your project is working, its valid. Slowly working your way up from a funtional starting base. My Project is currently 45-50% done. My next steps would be to add makers, center my map, and create a website around it including
- Directions
- Context
- Navigation tips
- Color and Decoration

I was able to get my map working by following this [guide I created](https://docs.google.com/document/d/18fefLc6nQL6y_yu4SGAUnliXsFcpn5lnHqkHvMBBpSg/edit?usp=sharing).
```JS
<!DOCTYPE html>

<html>

<head>

<title>Leaflet Web Map</title>

   <link
      rel="stylesheet"
      href="https://unpkg.com/leaflet@1.6.0/dist/leaflet.css"
      integrity="sha512-xwE/Az9zrjBIphAcBb3F6JVqxf46+CDLwfLMHloNu6KEQCAWi6HcDUbeOfBIptF7tcCzusKFjFw2yuvEpDL9wQ=="
      crossorigin=""
    />

    <script
      src="https://unpkg.com/leaflet@1.6.0/dist/leaflet.js"
      integrity="sha512-gZwIG9x3wUXg2hdXF6+rVkLF/0Vi9U8D2Ntg4Ga5I5BZpVkVxlJWbSQtXPSiUTtC0TjtGOmxa1AJPuV0CPthew=="
      crossorigin=""
    ></script>

<style>
#map {   
    width: 1350px;
    height:700px;
}
</style>

</head>

<body>

    <div id="map"></div>

<script>

    var map = L.map('map',{
    center: [40.6272, -74.0304], // coordantes set to Bayridge.
    zoom: 15 // set zoom of map
    });

    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(map);

</script>

</body>

</html>
```

### Lets break down the code.
1. Paste the long, scary links in the CSS and JS sections of your file. This will prep your file for what you want to code in the future. Its the building block of leaflet, and holds what you want to use. That was the first step. This took me a few tries at first, due to placement.
2. Create a DIV with the Id of map. put this in the location you want to have your map.
2.a In CSS, resize your map by using #Map to call it, and adjust the height accordingly.
3. The first essensial part of personalizng your map is setting the view. This is the automatic position your map will be in. It is the default coordantes your map rests on, such as being untouched or feshly loaded. One thing I would like to do in the future, would be to let the user input thier own coordnates. I gathered the coordnates for Bayride and set the map to there by using ``var map = L.map('map').setView([51.505, -0.09], 13);``. the command .setView litterally does what it says. It sets the default view of your map with the coordnates you provide in the parethisis following it.
3.a Setting the view of the map is another part of the default map. It is how zoomed in you want to be into the coordantes you chose above. I set the default zoom as 15 by using ``zoom: 15``. The zoom can be adjusted  by the user by using the provided buttons on the top left corner of the map.
4. The rest of the code is decalring coordantes and giving the map its ability to move, appear and follow the code written, simmilar to the links above.

[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)
