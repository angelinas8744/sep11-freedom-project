# Entry 2
##### 12/13/21

### Context
  The SEP11 freedom project gives me the oppurtunity to pick a coding language to create something I am passionate about. I decided on leaflet, a map making program to create a simple map website. I want to be able to help people find thier way around. I was thinking of having activities with some of its featues to help people of all ages get more famillair with thier surroundings. For example, I could have a alert to say mark all the bus stops pink, and all the train stations green, and give the user pink and green markers. Map markers are one of the features from leaflet. My goal is to create a website to support the user to feel comfortable and aware of where they are. Maps can be comfusing, and current sites can be complicated.

### What have I been working on ?
  On mondays, I have been reading and watching tutorials, mainly I try to stick with the same or simmilar sorces so I can memorize or reconize the code better. Seeing the repeating video's or articles is like studying for me. I have a good idea of how to create a base map because of this. To me, I think its important to start small, get good at that first, and then work my way up and bigger. I am currently working on reviewing how to create the map, since there is a lot to it, I have been spending the past weeks rewatching videos and following along, getting used to the code and the workflow of the coding language. As I go back and review, I know whats the next step, which helps me feel more confident and prepared for when its time to actually start. The start is most important because without a working map, set up correctly, you wont be able to do anything.
  
  However, I am not just sitting and watching. In my IDE, I made a planning page, which is a detailed step by step with example code.

### How am I learning?
  I am currently focusing on how to get the basics down to create a map. Watching youtube tutorials and reading articles. Another useful way was looking at github projects and reading the support questions people asked, such as errors and howw to fix them. With this information, I made myself a beginners guide on the topic. I took both pieces of code, expenations and step by step setups to help me start practicing leaflet. I wrote the directions in ways it easy for me to understand, and jotting idea's along the way, making me have all my thoughts in one place. Below, is what my planning page currently looks like.
```JS
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
To explain this, I started from the very beginning of creating a map. The first step is to put the code stated in CSS. And the same for the JS code. This prepares the page to be worked on further. Next, you add the div element where you want the map to be located, as well as its height. Next, you can set the view of your map. Finally, you have to add your map with the following code. The links that are in is for the example of london. You can change where the user starts off, with coordnates. You can also choose from different map types, with different types views or layouts. Once the map is up, you can set up tons of commands or extras for the user to customize and edit thier map, such as shapes, paths and markers.

### What is my plan ?
  Since starting a new map is a challanging and unfamiliar task, I have been hesitant to start practicing my code. In order to feel more prepared, I created my planning page as a reference to feel ready. Big code can be intimidating, especally if its new. I will take it slow, and not rush a perfect map all in one session. I will take one day for each step, so I can  really take the time to understand each part instead of rushing through just to get it to work. My plan of doing 1-2 steps thoroughly will help me get a clear understanding and will help me find what parts i need a better understanding on.

### What are some concerns ?
- Complex code that I havent learned yet
- Getting errors which will take me a while to fix
- fitting the map on the page along with text
- figuring out how to let the user input coordnates
      - a prompt and array?
- 

### What will I do next ?
- try new things !
- check out more github projects
- Keep track of all my trails, the success and errors.
- Continue to learn and ask questions.

#### How will I practice durring winter break?
My plan is to possibly begin my practice map. Since I have the time by myself, no bells or distraction. I can work for as long as I want, or even take breaks. I can follow along witha video if needed, and overall, its a more relaxed enviorment. My goal is to first get the map down, and then play with setting up its different features in class, since it takes less time and code (from what Ive seen). If I realize I need more support and things are still unclear while trying to code, I will take the time to watch those long, hour tutorials and take new notes, organizing my old ones, and writing example code. 

Overall, I think I have sucessfully progressed with my freedom project.

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
