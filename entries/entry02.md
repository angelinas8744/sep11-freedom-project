# Entry 2
##### 12/13/21

### Context
  The SEP11 freedom project gives me the oppurtunity to pick a coding language to create something I am passionate about. I decided on leaflet, a map making program to create a simple map website. I want to be able to help people find thier way around. I was thinking of having activities with some of its featues to help people of all ages get more famillair with thier surroundings. For example, I could have a alert to say mark all the bus stops pink, and all the train stations green, and give the user pink and green markers. Map markers are one of the features from leaflet. My goal is to create a website to support the user to feel comfortable and aware of where they are. Maps can be comfusing, and current sites can be complicated.

### What have I been working on ?
  On mondays, I have been reading and watching tutorials, mainly I try to stick with the same or simmilar sorces so I can memorize or reconize the code better. Seeing the repeating video's or articles is like studying for me. I have a good idea of how to create a base map because of this. To me, I think its important to start small, get good at that first, and then work my way up and bigger. I am currently working on reviewing how to create the map, since there is a lot to it, I have been spending the past weeks rewatching videos and following along, getting used to the code and the workflow of the coding language. As I go back and review, I know whats the next step, which helps me feel more confident and prepared for when its time to actually start. The start is most important because without a working map, set up correctly, you wont be able to do anything.
  
  However, I am not just sitting and watching. In my IDE, I made a planning page, which is a detailed step by step with example code.

### How am I learning?
  I am currently focusing on how to get the basics down to create a map. Watching youtube tutorials and reading articles. Another useful way was looking at github projects and reading the support questions people asked, such as errors and howw to fix them. With this information, I made myself a beginners guide on the topic. I took both pieces of code, expenations and step by step setups to help me start practicing leaflet. I wrote the directions in ways it easy for me to understand, and jotting idea's along the way, making me have all my thoughts in one place. Below, is what my planning page currently looks like.
```
 How to ADD leaflet

https://www.tutorialspoint.com/leafletjs/leafletjs_getting_started.htm

map startup requirements:
1. An html page
2. The Leaflet CSS styles
3. The Leaflet JavaScript library
4.A <div> element to hold the map
5. A height style specified for the map div.
6. A short script to create the map in that <div>

- you can create pathways and mark routes with a line funtion
use shapes to mark or highlight routes or areas
- erase tools
- dot markers
example : https://stephsaephan.github.io/leaflet-map-example/

steps !
------------------------css paste first --------------------------
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css"
   integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A=="
   crossorigin=""/>
-------------------------- Java Script after CSS-------------------------
<script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js"
   integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA=="
   crossorigin=""></script>
--------------------------- Div element for map, where you want it.--------------------
 <div id="map"></div>

and add height -    #map { height: 180px; }
----------------------------- Setting the view for the map. --------------------------
var map = L.map('map').setView([51.505, -0.09], 13);
                                  ^ coordnates for set view


The example is set to london. ypu can either...
1. make it set to tele
2. set to a user input.
   - get coordentes by prompt and put it into map.


! map of bayridge !

----------------------
map view of ZERO : (256 pixels wide and 256 pixels high)

var map = L.map('map', {
    minZoom: 0,
    maxZoom: 0
});

var cartodbAttribution = '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors, &copy; <a href="https://carto.com/attribution">CARTO</a>';

var positron = L.tileLayer('https://{s}.basemaps.cartocdn.com/light_all/{z}/{x}/{y}.png', {
    attribution: cartodbAttribution
}).addTo(map);

map.setView([0, 0], 0);

------------------ adding markers ---------------

   var marker = L.marker([51.5, -0.09]).addTo(map);

   idea: add markers for each trainstation of bayridge blue and bustops green / red depending on the line and where its stops are

---------------- adding popups ---------------------
marker.bindPopup("<b>Hello world!</b><br>I am a popup.").openPopup();


---------------- tells you where you clicked ---------------
var popup = L.popup();

function onMapClick(e) {
    popup
        .setLatLng(e.latlng)
        .setContent("You clicked the map at " + e.latlng.toString())
        .openOn(map);
}

map.on('click', onMapClick);

this will give a popup for the user to tell them the coordates of where they are.
```
To explain this, I started from the very beginning of creating a map. The first step is to put the code stated in CSS. And the same for the JS code. This prepares the page to be worked on further. Next, you add the div element where you want the map to be located, as well as its height. Next, you can set the view of yoyr map. Finally, you have to add your map with the following code. The links that are in is for the example of london. You can change where the user starts off, with coordnates. You can also choose from different map types, with different types views or layouts. Once the map is up, you can set up tons of commands or extras for the user to customize and edit thier map, such as shapes, paths and markers.

### What is my plan ?

### What are some concerns ?

### What will I do next ?

#### How will I practice durring winter break?



Text

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
