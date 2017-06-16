---
layout: default
title: PowerBI - Routemap Custom Visual
image_sliders:
  - slider1
---

[comment]: # (checklist: )
[comment]: # (a. _data/sliders.yml: change the images)
[comment]: # (b. _incudes/disqus_comments.html: change the forum id)
[comment]: # (c. index.md: title and content)

# Background
This is a custom visual built for PowerBI to support rout visualization. Route map basically visualizes trajectories of objects, such as taxies, vessels, airplanes, and hurricanes.

{% include slider.html selector="slider1" %}

# Where to Get It

You can get it from the [_Office Store_](https://store.office.com/en-us/app.aspx?assetid=WA104380985&sourcecorrid=95716b6f-f393-4115-9447-5bbfa5b95537&searchapppos=0&ui=en-US&rs=en-US&ad=US&appredirect=false) or in the [_dist_](https://github.com/weiweicui/PowerBI-Routemap/tree/master/dist) folder of this [_repo_](https://github.com/weiweicui/PowerBI-Routemap).

# How to Use
* Required fields: 
    * **Timestamp**: Values in this field are used to decide the chronological order of the records. These values can be anything sortable, such as numbers and dates.
    * **Latitude** and **Longitude**: Geo-coordinates for the records. 
* Optional fields:
    * **Segment**: Records are grouped into routs based on this field. If not specified, all records are connected together.
    * **Color/Width/Dash Legend**: If specified, you can customize the route styles in the _Format_ tab.
    * **Tooltip**: Values here will be displayed when hovering over route arrows.

* Special settings:
    * **Legend**: You can customize labels for colors, widths, and dash types. If the labels are empty, they will not show in the legend.
    * **Arrow** - **Interval**: This controls the sparseness of arrows. Too many arrows may cause visual clutter and slow down the performance.
    * **Dash**: There are several dash types available. However, drawing very long dashed lines may slow down your browser.
    * **Advanced** - **Ignore zeros** and **Ignore invalids**: These are two simple safeguards of the visual. If geo-locations are all zeros, i.e., _(0,0)_, or invalid, i.e., _abs(latitude) > 85.05112878 or abs(longitude) > 180_, they will be excluded from the visual. These two switches are on by default.
    
* Need more help? Please leave a comment below.