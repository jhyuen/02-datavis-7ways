Assignment 2 - Data Visualization, 7 Ways  
===

Author
---
Joseph Yuen

Project Description
---
I used the following set of libraries, tools, and languages to recreate the same chart based on the cars-sample.csv.

1. d3
2. Flourish
3. Vega-lite
4. R + ggplot2
5. Tableau
6. GNUplot
7. Matplotlib

Some more words about the process and how I did it.

Libraries, Tools, Languages
===

d3
---
### Discussion
It was hard

### Image
![Screenshot1](img/.png)

Flourish
---
### Discussion
It was hard

### Image
![Screenshot1](img/.png)

Vega-lite
---
### Discussion
It was hard

### Image
![Screenshot1](img/.png)

R + ggplot 2
---
### Discussion
It was hard

### Image
![Screenshot1](img/.png)

Tableau
---
### Discussion
It was hard

### Image
![Screenshot1](img/.png)

GNUplot
---
### Discussion
It was hard

### Image
![Screenshot1](img/.png)

Matplotlib
---
### Discussion
It was hard

### Image
![Screenshot1](img/.png)




Achievements
===
## Technical
1. **Hover** - I implemented mouseover and mouseout events in combination with transitions to change the color of shapes upon hovering over them. In addition, id selectors to identify certain groups of shapes that required a different style to be changed. For example, some circles, required the stroke to be changed and the not the fill. In the picture below, I show what happens when the user hovers over a section of the bike.

2. **Rotation Animation** - Upon entering the webpage, the wheels on the bike rotate clockwise. I accomplished this effect by using a d3.timer that loops based on real time. Initially, I tried using a transform in a transition, but I realized that I needed to calculate the previous angle of each wheel to keep the wheel rotating in place. Before, the wheel would rotate and move around instead of rotating and remaining in place.

3. **Re-sizeable Viewport** - I initially made the bike using the vw and vh units unaware that d3 uses the viewBox attribute to scale their graphs. Certain primitives like polygons didn't take vw and vh as inputs which forced me to redo my shapes using a viewBox attached to the svg object. By using viewBox, shapes and text are automatically resized forced to maintain a 1920x1080 aspect ratio as seen in the picture below.

## Design
1. **Bike** - Based on the reference picture below, I created a simplified version of the bike using primitive shapes instead of just drawing a couple shapes on a canvas.

Resources
===
