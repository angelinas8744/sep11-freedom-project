# Entry 3
##### 2/10/22
### Learning Process
  My biggest solution to everything is writing it out. No matter what it's for, I write it out. I decided to do the same for all the new Information about coding with Leaflet. At first, I had a messy folder in my IDE, but I decided to write down all of my takeaways on a google doc. This includes steps, resources and general tips of creating maps with leaflet, and any functions or add ons you want it to have. I find things stick better when I keep rewriting it or rewatching the same resource. Making this document helped me organize my information, as well as getting more familiar with the workflow. My document is still under construction, but it can be viewed [here.](https://docs.google.com/document/d/18fefLc6nQL6y_yu4SGAUnliXsFcpn5lnHqkHvMBBpSg/edit?usp=sharing)
  ### The Biggest Setback
  The current challenge right now is gathering enough information, as well as feeling confident enough to start practice. Since Leaflet requires an active map to code on, I would first have to spend my time creating a map, then what I want it to do. I can try out different features such as custom markers. Being able to look at examples of websites lets me find what I like and don't like and then know what I wanna include and what code I need. But to do this, I would first need to make a base map website. I plan to have started creating this map by my next blog. I will spend the time in between really focusing on preparing, and building myself up to start the base. To me, Leaflet seem like dominoes. First is the map, then everything else falls in place. I also have to take into consideration trial and error. I tend to get stnervus or discouraged with errors, so feeling ready is just as important as having the material. This is the skill of patience, which coding has slowly taught me, as well as not fearing mistakes. Although I may not be the best at that as we speak, I plan on facing that bigger issue this month. Taking that leap not only applies to coding, but plenty of situations in life.
 ### What is my plan?
 1. Every monday, repeat one [tutorial](https://youtu.be/wVnimcQsuwk) to gain a consistent familiarity with the process.
 2. Continue to add to and revise my google doc, making a clear step by step to best avoid errors and intimidation.
 3. Get the base map done.
 4. Do further research on what to add to it, and how to make it interactive.

One thing you can add to leaflet is markers. These will mark a location on your map. You can have pre-set ones, or ones added by the user.
```
var marker = L.marker([51.5, -0.09]).addTo(map); 
var popup = marker.bindPopup('<b>Hello world!</b><br />I am a popup.'); 
```
  > idea: add markers for each trainstation of bay ridge blue and bus stops green / red depending on the line and where its stops are.
   
 6. Possibly use content learned in class such as DOM events, if they work with the code.
 7. Look at leaflet github projects and try them out, see what features are liked and disliked, and do further research.
 8. Add and play around with them in my sandbox map.
 9. Plan out what content I want around my map, and what I want the website to look like.


### One question I have that still is unanswered is..
 I noticed in one guide you needed a a text or code editor, which I wonder what this is? They gave the example of Sublime Text, Atom Editor, or Visual Studio Code.
After researching, I noticed sublime text has to be downloaded. Is it required for coding leaflet?

### How would I explain this to beginners?
- Start by building up from the map
- Take small steps
- Don't intimidate yourself with big articles

Leaflet is a pretty straightforward Javascript Library. From what I've learned, It's like building blocks. Its very step by step. I would recommend to my past self, or somebody learning this to follow each step, one at a time. I would reccoemned to not move on to the next step until you really focused on and understand the previous one. 

### Tips and goals for my future self.
1. Try out everything you learned.
2. Mistakes will tell you what you need to learn more.
3. If you're confused on a step, go back and study it more.
4. Try One step per day, really focusing on writing it and understanding it, not just to get it to work.
5. Learn more about my question.
6. add more interactive methods once I try to get a base map running.


[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)
