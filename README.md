# UFO Sightings Visualization

<img src="img/full_project.png">

**FIGURE 1.** An overall look at the project and its visualizations.



### THE PROJECT


**Maps:** [UFO Sightings Maps](https://bridgethaney.github.io/UFO_Sightings_Project/)

**Data:** [UFO Sightings Dataset](https://data.world/timothyrenner/ufo-sightings) by Tim Renner


### INTRODUCTION

Extraterrestrial life has been long debated and examined through scientific research, eyewitness testimony, and pop culture. One of the most prominent ways this exploration of possible alien contact has occured is through sightings of unexplainable phenomenon detailed as unidentified flying objects. According to the National UFO Reporting Center, there have been over 5,971 sightings of UFOs in 2019 in North America (Pereira, 2020). With the noticeable prevalence of UFO sightings within North America and in particular, the United States, it is worth an investigation into the frequency of UFO sightings and where the largest amount of sightings occur.

The previous acting Director of National Intelligence, Richard Grenell, has stated that there have been instances, in fact, of UFOs. 

Surprisingly, along with this data advancing scientific research, there is also a deeper rooted effect to seeing UFOs. It is shown that the "68% today who believe the government is withholding information about UFOs is comparable to the 71% found in 1996" (Saad, 2021). This means that due to possible UFO sightings, individuals may believe that the government is not being transparent or hiding information about UFOs or possible alien life, which signifies that there is some sort of distrust in the government surrounding this topic.


### PROJECT GOAL

This featured visualization seeks to find any patterns within sightings of three different locations: the Greater Los Angeles Area, Albuquerque, New Mexico, and the Greater New York City Area. There is a common conception that the crash site of a UFO located within Roswell, New Mexico, is the hub for alien activity. This makes Albuquerque, the biggest city closest to Roswell, the perfect location to test whether surrounding areas to Roswell have the highest amount of sightings, or if other locations, like Los Angeles do. Through focusing on several different locations, there can ultimately be a wider look into where UFO sightings are most prevalent. It is interesting to see just how many UFO sightings are reported, the description of each UFO sighting, and the kinds of shapes that UFOs can take form through. 

* Area 51 in Nevada will also be added in.

**Audience:** Ufologists are the prime target for this research. A Ufologist is an individual that specifically studies and identifies . 

### ANALYSIS

In observing the data in all three locations, it seems that New York City contains the most sightings. This could be due in part to the expansiveness of the city and situational factors, like heavy airport traffic. It seems in bigger cities, there are in general, more sightings. 

### TECHNICAL OVERVIEW


- **UFO Sightings Map**
    - Layers
        - Basemap: Customized Monochrome Basemap made on MapBox
        - Thematic layer: UFO Sightings Data with colors of symbols changing based on shape type of UFO
        - Basemap w/ Thematic Layer: Combines both the basemap and UFO data for ease of access
    - Libraries / Packages
        - Leaflet: Creates the maps
        - QMetaTiles: Package on QGIS that converts maps to 256 pixel tiles

- **Methodology and Steps**
    - First, the basemap was created within Map Box. The base colors were darker grays, while location labels and streets were given light blues, greens, yellows, and oranges depending on zoom.
    - The thematic layer was then acquired. The UFO dataset by Tim Renner, which is found on the website data.world, contains information on UFO sightings. On the map, the data points are represented by circles that are color coordinated to the shape of the UFO sighted.
    - The basemap, thematic layer, and both the basemap and thematic layer together are converted to 256 pixel tiles through QMetaTiles on QGIS. This allows for visually-appealing design and more quick display of information.
        
- **Resources:**
    - [UFO Sightings Dataset](https://data.world/timothyrenner/ufo-sightings) by Tim Renner
    - [Three Maps on Leaflet](https://stackoverflow.com/questions/52597399/displaying-3-leaflet-maps-on-same-page) as explained by Marat Badykov


### GUIDE

#### **New York City Map**

<img src="img/new_york_sightings.png">

**FIGURE 2: Static image of the interactive leaflet map featuring New York City UFO sightings**

#### **Albuquerque Map**

<img src="img/albuquerque_sightings.png">

**FIGURE 3: Static image of the interactive leaflet map featuring Albuquerque UFO sightings**

#### **Los Angeles Map**

<img src="img/los_angeles_sightings.png">

**FIGURE 4: Static image of the interactive leaflet map featuring Los Angeles UFO sightings**

#### **Legend: Shapes of UFOs**
   - Each UFO shape is represented by a color symbol on the map
   - There are 21 shapes featured in the data
   - The types of shapes are: Love, Changing, Chevron, Circle, Cone, Cross, Cylinder, Diamond, Disk, Egg, Fireball, Flash, Formation, Light, Other, Oval, Rectangle, Sphere, Teardrop, and Triangle
    
<img src="img/ufo_shapes_legend.png">

## Acknowledgements

Some code snippets are taken from the UW GEOG 458 Lab 4 assignment by Bo Zhao. I am also using some formatting code from Marat Badykov on Stack Overflow to create the three maps.

## References

Saad, L. (2021, January 14). Americans Skeptical of UFOs, but Say Government Knows More. Retrieved from https://news.gallup.com/poll/266441/americans-skeptical-ufos-say-government-knows.aspx

Pereira, I. (2020, January 8). UFO sightings in North America jumped to nearly 6,000 in 2019. Retrieved March 16, 2021, from https://abcnews.go.com/US/ufo-sightings-north-america-jumped-6000-2019/story?id=68145474


