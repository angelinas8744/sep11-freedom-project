# Entry 5
##### 4/25/22

Wow! I finally hit the milestone of finishing my MVP. I feel like it was just yesterday that I was picking Leaflet and started off the year. I was so worried I would struggle or mess up but everything went smooth and according to plan! 

Lets start with what I left off from my last blog. I was able to finish the basics, as the *tough* extension of adding default markers. I was able to put one on HSTAT, one on the B4 bus stop, and one on the R train station. Coloring the markers was a dificult task I wasnt able to reach because I would have to download leaflet markers and attach them to my IDE. **My next step**, beyond MVP would be to add text to the markers, as well as a smaller weather map below the mail sattelite one.

Well, time to show off the finished MVP ive been talking about!

### Part 1. Code Breakdown.
 ```
 <!DOCTYPE html>

<html>

<head>
<h1>Welcome to My Leaflet map. Move around by clicking and dragging. Zoom in by double clicking or using the provided zoom buttons.</h1>
<p> Navigation can be tricky. Especally when maps are becoming high tech, and you start to memorize directions less, and have computers do it for you. Here, You can use a basic map to navigate around. Here are some tips for getting to know your routes. Like everything in life, it takes practice.</p>
<li> Find the easiest and most effective route </li>
<li> Review it, from start to end, back and forth until you have it down. </li>
<li> Slowly make changes in that route, such as turning down a differnt block. </li>
<li> Find more routes. </li>
<li> Study street signs and see its patterns, such as which directions the numbers increase or decrease. </li>
<li> Repeat this method with different Locations around !</li>
<br>
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
    width: 2530px;
    height:950px;
}

body {
background-color: #DBF9FC;
}

h1{
 color: #0099FF;
}

p{
 font-size: 25px;
 color:#6a0dad;
}

li{
 font-size: 25px;
 color:#0099FF;
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

  var markerhstat = new L.marker([ 40.6366386,-74.0229627]); // HSTAT marker
   var markerb4 = new L.marker([ 40.630641, -74.024689]); // B4 stop 75th and 4th
   var markerRtrain = new L.marker([ 40.6349359,-74.0234975]); // R train station
   /// Adding the markers above to map.
   markerhstat.addTo(map);
   markerb4.addTo(map);
   markerRtrain.addTo(map);
   ```
   Looks like a lot of code right? Well, working with Leaflet is a big step by step process. This is the big picture, lets break down each piece.
   
   1. The first thing you probally noticed, like me, was all of the weird links. This is to setup Leaflet to be used, and what map you want to show up on your page.

</script>

</body>

</html>

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
