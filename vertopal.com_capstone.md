---
title: "*capstone-case-study-cyclystic*"
---

**overall goal of the study**

-Maximizing the annual membership by converting the casual rider into
annual members

**key focus**
![day of the week count total pivot table](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/fcd66ddc-3026-4777-88af-b8f895eb0fca)

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
<img src="capstone-case-study-cyclystic
/table for total ride on each day for each month.png">

-calculate the total rides each month by customers\
-used pivot table to construct the result table\
insert image here

-calculate the total rides each month by subscribers\
-used pivot table to construct the result table\
insert image here

-calculate the count for how many times customers start riding from each
station for jan,feb, marc

-filtered to see the hotspot above 500 count to see the popular starting
location

used pivot table to construct the result table\
insert image here

-calculate the count for how many times customers start riding from each
station for april,may,june

-filtered to see the hotspot above 3000 count to see the popular
starting location

used pivot table to construct the result table\
insert image here

**Phase -- 5 Share**
