4/25/22
Wow! I finally hit the milestone of finishing my MVP. I feel like it was just yesterday that I was picking Leaflet and started off the year. I was so worried I would struggle or mess up but everything went smoothly and according to plan!
Let's start with what I left off from my last blog. I was able to finish the basics, as the tough extension of adding default markers. I was able to put one on HSTAT, one on the B4 bus stop, and one on the R train station. Coloring the markers was a difficult task I wasn't able to reach because I would have to download leaflet markers and attach them to my IDE. My next step, beyond MVP would be to add text to the markers, as well as a smaller weather map below the mail sattelite one.
Well, time to show off the finished MVP I've been talking about!
Part 1. Code Breakdown.
<!DOCTYPE html>

<html>

<head>
<h1>Welcome to My Leaflet map. Move around by clicking and dragging. Zoom in by double clicking or using the provided zoom buttons.</h1>
<p> Navigation can be tricky. Especially when maps are becoming high tech, and you start to memorize directions less, and have computers do it for you. Here, You can use a basic map to navigate around. Here are some tips for getting to know your routes. Like everything in life, it takes practice.</p>
<li> Find the easiest and most effective route </li>
<li> Review it, from start to end, back and forth until you have it down. </li>
<li> Slowly make changes in that route, such as turning down a different block. </li>
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
   center: [40.6272, -74.0304], // coordinates set to Bayridge.
   zoom: 15 // set zoom of map
   });


   L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
   attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
   }).addTo(map);

 var markerhstat = new L.marker([ 40.6366386,-74.0229627]); // HSTAT marker
  var markerb4 = new L.marker([ 40.630641, -74.024689]); // B4 stop 75th and 4th
  var markerRtrain = new L.marker([ 40.6349359,-74.0234975]); // R train station
  /// Adding the markers above to the map.
  markerhstat.addTo(map);
  markerb4.addTo(map);
  markerRtrain.addTo(map);
 
Looks like a lot of code right? Well, working with Leaflet is a big step by step process. This is the big picture, let's break down each piece.
The first thing you probably noticed, like me, was all of the weird links. This is to set up Leaflet to be used, and what map you want to show up on your page. Following, You must put <div id="map"></div> between body and script. Small errors in the placement- the hardest part of the coding, its setup- will lead to problems with the map and its code. The setup took a good two tries.
Next, Is the start of the map itself. First, you want to set up var map = L.map which holds the map itself, allowing you to call it multiple times as needed and add new things. L. is used through Leaflet. In addition to holding the map, you need to tell the page the dimensions and default zoom, as well as the default coordinates. I set the coordinates to Bayride, enough to get a good overview of the area. The zoom and coordinates are done in the JS section in the map variable. center stands for the center coordinates, or middle coordinates of the default map. Zoom, is how close or far you are from the location, the closer, the more specific view you get. You can alway adjust the zoom and coordinates manually on my site. Unlike the other two setups, the map dimensions have to be done in CSS because it is considered the style of the map, and does not affect how it functions. You can have the map any look possible and it will always work the same. It is more considered the looks, but it is mandatory for it to appear.
Next, we hit L.tileLayer. This gives the map its satellite look. You can choose from many map types. You copy and paste the given link, sourcing the map to know how to look, and then .addTo(map);.
keep in mind .addTo(map); comes up a lot in leaflets. It works like git push, it adds and commits changes to your map, and saves the new information to it!
Now, you have a basic map. By now, I had about a month left. I was able to learn and create three basic markers, and try to learn how to edit them once placed ( but didn't get the chance to finish- therefore working on it as a beyond MVP ). For the standard basic marker, you need coordinates and variables. new L.marker creates a new marker rather than overlapping the coordinates on one marker, allowing only one. you need to call a new marker for each one, making them distinct from one another. Here is an example of how a marker should look. var markername = new L.marker([ X,Y]);
Finally, you have to add each marker to the map by first calling the marker's name followed by .addTo(map);.
Part 2. The Product.
Part 3. Improvements.
My priority for improving my map is the makers. They currently look identical. The markers are definitely more complicated when you want to edit them. You need to create seperate vars and learn lots of new commands, as well as downloading fitting markers for each different one you want, such as a pencil for school, or a simple green one. The default leaflet marker is currently on my map. My second task would be a smaller weather map. I am interested in this because of the similar and different features, code, and it looks really cool overall. This can track rain, temperature or snow, using colors over a location.
Part 4. Takeaways and Achievements.
Order matters, as well as placement in code.
Simple code can be hard, Hard looking code can be simple.
Tasks can be easier than they look.
The longer you wait, the more worried you will be about the outcome
You will never find the perfect guide, take what sticks out to you from different ones and create your own! This was extremely helpful when it came to this project.
Pay attention to dates on guides, as outdated ones will be useless.
Time management skills, self motivation and using guides responsibly.

</script>

</body>

</html>

[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)
