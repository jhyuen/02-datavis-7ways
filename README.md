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
4. R+ggplot2
5. Tableau
6. Excel
7. Matplotlib

Some more words about the process and how I did it.

Libraries, Tools, Languages
===

d3
---
### Discussion
d3 is a JS library that gives the user low level tools to create visualizations based on data. 

In my implementation, I created the axis and then added data points in the fetch to the csv file. When collecting the points, I added functions that changed the color of circles based on their manufacturer. 

I thought that d3 was the most difficult of the tools as it gave the most customization. However, the higher difficulty can be worth it as d3 can produce complex visualizations that have truly unique interactions. For example, it was  annoying to move the circles separately from the axis. In addition, it was strange to add a title to each of the axis. Most of the programs I used had an automatic feature to create an axis title. But even so, I see why d3 does this as to give more freedom to the developer.

### Screenshots
![d3](img/d3-1.png)

Flourish
---
### Discussion
Flourish describes itself as a "CMS for interactive content." It is a data vis online software that makes it easy for people to make complex visualizations with no coding necessary. I think of it as a simpler version of Tableau for those who have little data experience.

The program has the user first load in their data and then has them fill out the x, y, size, and color information. I found this setup to be relatively simple as it produced a graph very close to the end product in a matter of minutes. I then spent most of my time editing the axis to make sure I had the right intervals.

As I've said before, I found the program to be really simple to adopt and can see myself using it in the future for quick and casual visualizations. I also will likely suggest it to peers who do not code and are new to making visualizations.

Link to Project:
https://public.flourish.studio/visualisation/5379670/

### Screenshots
![Flourish](img/flourish-2.png)
![Flourish - edit interface](img/flourish-1.png)
![Flourish - data interface](img/flourish-3.png)

Vega-lite
---
### Discussion
Vega-lite is a "high-level grammar" for data visualizations. It provides a relatively easy to follow syntax that automatically produces many necessary objects such as axis and legends.

To make this scatter plot, I examined JSON implementations of scatter plot examples and then converted it into a JS implementation with the correct values. When writing the JS, I only had to define the x axis, y axis, circle color, and circle size with a couple lines of codes. Everything else was taken care of automatically.

Vega-lite in its JSON implementation is straight forward and relatively easy to use. My biggest difficulty was converting the JSON into JS. I can see it being a tool for data scientists with a minimal understanding of programming to communicate data quickly. However, there's not too many customization options for aesthetics which may prevent it from being used for general audiences that likely want more aesthetically pleasing visualizations.

### Screenshots
![Vega-lite](img/vega-lite.png)

R + ggplot 2
---
### Discussion
ggplot2 is a statistics and data vis library for the coding language R. It is commonly used with RStudio to provide users with an easy to use interface that shows existing variables and graph output. 

I looked at some implementations of ggplot2 to get started and was able to write the entire graph in about 3 lines of code. Since the default picture was made in ggplot2, they are almost identical. 

I found that ggplot2 was relatively easy to code, but I found setup to be  annoying. When I downloaded the ggplot2 package, it kept requiring me to download dependencies that wouldn't download. Eventually, I moved to using RStudio within Anaconda for package management. When I used RStudio to add packages, I had the same issue. I realized I had to download the packages through Anaconda. And even though I could download new packages in Anaconda, I still had to download the many dependencies for ggplot2 to run. For that reason, I wouldn't recommend this to a new data vis user. I see this library similarly to Vega-lite which requires a little more coding knowledge and can be used for quick and informative graphs.

### Image
![r-ggplot2](img/r-ggplot2-1.png)
![r-ggplot2 - edit interface](img/r-ggplot2-2.png)

Tableau
---
### Discussion
Tableau is a popular no coding required (although you can code for custom features) data vis tool. It offers many hover and filter features that can be used to make interactive dashboards.

To make the scatter plot, I loaded the data into Tableau and then assigned the rows (y-axis) and columns (x-axis) with the appropriate data. Then I defined the circles' color and size by selecting a couple drop down menus, and in minutes I had a fully functional data vis with hover features over each data point.

I thought that Tableau was simple to use as I did not have to use any sort of tutorial. However, I think that it can be intimidating for users less familiar data. It is more complex than Flourish, but it also offers many more features. The benefit of Tableau is that it can be used to make both quick and complex aesthetically pleasing visualizations with no coding required.

### Screenshots
![Tableau - edit interface](img/tableau-1.png)
![Tableau](img/tableau-2.png)

Excel
---
### Discussion
It was har


Write a paragraph for each visualization tool you use. What was easy? Difficult? Where could you see the tool being useful in the future? Did you have to use any hacks or data manipulation to get the right chart?

### Screenshots
![Excel](img/excel-1.png)
![Excel - edit interface](img/excel-2.png)

Matplotlib
---
### Discussion
It was hard

### Screenshots
![Matplotlib](img/matplotlib-2.png)
![Matplotlib - edit interface](img/matplotlib-1.png)

Achievements
===
## Technical
1. **NA Handling** - As libraries such as ggplot2 automatically eliminated Weight MPG pairs with NA values, I eliminated rows that had NA values in MPG. By doing so, all of my graphs looked the same as some libraries caused NA values to either default to 0 or mark at the top of my graph. 
2. **Extra Library** - Even though the base requirement was to use 3 libraries, I used an additional library to total 4 libraries: Matplotlib (Python), ggplot2 (R), d3 (JS), and Vega-lite (JS).
3. **Maintained Aspect Ratio for d3** - I wrapped my d3 implementation in a viewBox with a 1920x1080 aspect ratio. As a result, my points and text automatically scale down as the window becomes smaller.
4. **d3 Hover** - Devoted tools like tableau offered a feature that allowed the user to hover over a point and get more information on it. I implemented a similar functionality in d3. !!!NEED TO DO!!!

## Design
1. **Design Achievement 1** - Description
Create legends for missing ones
Match colors?

Resources
===
Vega-Lite: https://vega.github.io/vega-lite/tutorials/getting_started.html#tutorial-overview

R-ggplot2: http://r-statistics.co/Complete-Ggplot2-Tutorial-Part1-With-R-Code.html