---
title: "*capstone-case-study-cyclystic*"
---

**overall goal of the study**

-Maximizing the annual membership by converting the casual rider into
annual members

**key focus**

-How to understand casual riders and annual members use cycllystic
differently

**The Plan(Overview)**

-is for the team to create a new marketing strategy to convert casual
riders into annual members

**What is cyclystic**

-Cyclystic is abike sharing program that has cycling bikes,hand
tricycles, and cargo bikes.the comapny is based in chicago, it has 692
station where it has 5,824 bicycles

-They have two type of riders

**casual rider**

which has two modes:

-\> single ride pass

-\>full day pass

**annual members**

-purchases a annual membership

-30% of the users commune to work using cyclystic bicycles

Phase 1 - Ask

-How do annual members and casual riders use cyclystic bike differently?

**The Problem**

-We have two type of riders casual and annual member, only one side is
more profitable than the other, which mean their amount of usage is
diffferent

**The business task statement**

in cyclystic, there are two type of riders, annual and casual, we are
tasked to find out and analyze how the casual and annual user use
cyclystic differently, based on that analysis we will find trends and
realtionships that can help us convert casual into annual membership
subscribers and boost the companies future sucess

**Key stakeholders**

1.Cyclystic executive team

2.Lily moreno

3.marketing analytic team

**Phase 2 - Prepare**

-Dataset Chosen is the Divvy_trip 2017 for the 6 month which includes
January, February, march, April, May and June

-The dataset is located at motivate international Inc.

-The data is organized in quarterly manner

-The licensing is given by Divvy on their divvy data license agreement

Tools of choice:

-Excel

-Rstudio\
-Tableu

**Phase 3 -- Process**

-added another timeduration(minutes) column from that converted the
timeduration column from seconds to minutes\
Formula used:=\[@\[tripduration\]\]/(60\*60\*24)

-Changed the names of the from_station_name and to_station_name into
starting_station and ending station

-Extract the day from starting_time and added it into new column called
starting day

Formula used: =Text(c2,"dddd")

\- Extract the month from starting_time and added it into new column
called month

Formula used: =Text(c2,"mmmm")

**Phase 4 -- Analysis**

-calculate the total rides on each day for each month of the dataset

-used pivot table to construct the result table\
![table  for total ride on each day for each month](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/60b840d8-453f-406e-81b4-315b83a542a1)


-calculate the total rides each month by customers\
-used pivot table to construct the result table\
![table total rides of customer each month](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/7c79c16d-5b67-4df3-8a65-73c698944af9)


-calculate the total rides each month by subscribers\
-used pivot table to construct the result table\
![table for total ride each moth by subscriber](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/bfd77324-6e2d-4a67-859c-d5915ca74f44)


-calculate the count for how many times customers start riding from each
station for jan,feb, marc

-filtered to see the hotspot above 500 count to see the popular starting
<div class='tableauPlaceholder' id='viz1700702727599' style='position: relative'><noscript><a href='#'><img alt='Sheet 1 ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;ho&#47;howmanycustomerstartedfromstartstateionabove500q1&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='howmanycustomerstartedfromstartstateionabove500q1&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;ho&#47;howmanycustomerstartedfromstartstateionabove500q1&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-GB' /><param name='filter' value='publish=yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1700702727599');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

used pivot table to construct the result table\
insert image here

-calculate the count for how many times customers start riding from each
station for april,may,june

-filtered to see the hotspot above 3000 count to see the popular
starting location

used pivot table to construct the result table\
insert image here

**Phase -- 5 Share**
