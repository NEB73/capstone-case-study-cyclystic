---
title: "*capstone-case-study-cyclystic*"
---

<br>**overall goal of the study**

-Maximizing the annual membership by converting the casual rider into
annual members

<br>**key focus**

-How to understand casual riders and annual members use cycllystic
differently

<br>**The Plan(Overview)**

-is for the team to create a new marketing strategy to convert casual
riders into annual members

<br>**What is cyclystic**

-Cyclystic is abike sharing program that has cycling bikes,hand
tricycles, and cargo bikes.the comapny is based in chicago, it has 692
station where it has 5,824 bicycles

-They have two type of riders

<br>**casual rider**

which has two modes:

-\> single ride pass

-\>full day pass

<br>**annual members**

-purchases a annual membership

-30% of the users commune to work using cyclystic bicycles <br>

**Phase 1 - Ask**

-How do annual members and casual riders use cyclystic bike differently?

<br>**The Problem**

-We have two type of riders casual and annual member, only one side is
more profitable than the other, which mean their amount of usage is
diffferent

<br>**The business task statement**

in cyclystic, there are two type of riders, annual and casual, we are
tasked to find out and analyze how the casual and annual user use
cyclystic differently, based on that analysis we will find trends and
realtionships that can help us convert casual into annual membership
subscribers and boost the companies future sucess

<br>**Key stakeholders**

1.Cyclystic executive team

2.Lily moreno

3.marketing analytic team

<br><br>**Phase 2 - Prepare**

-Dataset Chosen is the Divvy_trip 2017 for the 6 month which includes
January, February, march, April, May and June

-The dataset is located at motivate international Inc.

-The data is organized in quarterly manner

-The licensing is given by Divvy on their divvy data license agreement

Tools of choice:

-Excel

-Rstudio\
-Tableu

<br><br>**Phase 3 - Process**

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
<br>
Then to combine all of the datasets of excel files which were in csv format i used R studio the code for the combination of the csv files is below <br><br>
``` 
inputfiles = c("D:/casestudy cyclystic/Divvy_Trips_2017_Q1Q2")
new_data=data.frame()


for(inputfile in inputfiles){
  data = read.csv(inputfile,header = FALSE)
  new_data<-rbind(new_data,data)
}
```

<br><br>**Phase 4 - Analysis**

1.)calculate the total rides on each day for each month of the dataset

-used pivot table to construct the result table <br>
![table  for total ride on each day for each month](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/60b840d8-453f-406e-81b4-315b83a542a1)<br>

2.)calculate the total rides each month by customers\
-used pivot table to construct the result table\
![table total rides of customer each month](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/7c79c16d-5b67-4df3-8a65-73c698944af9) <br>


3.)calculate the total rides each month by subscribers\
-used pivot table to construct the result table\
![table for total ride each moth by subscriber](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/bfd77324-6e2d-4a67-859c-d5915ca74f44)<br>


4.)calculate the count for how many times customers start riding from each
station for jan,feb, marc

-filtered to see the hotspot above 500 count to see the popular starting
used pivot table to construct the result table\
![count of customers starting point to ride a bicycle above 500 for jan,feb,mar](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/88355168-3ac3-431a-8567-148e65c87ce4)<br>


5.)calculate the count for how many times customers start riding from each
station for april,may,june

-filtered to see the hotspot above 3000 count to see the popular starting location
used pivot table to construct the result table\
![count of customers starting point to ride a bicycle above 3000 for may, june,jul](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/f775f738-fa9a-45c0-8859-d689a51e7e2d)<br>




**Phase - 5 Share**<br><br>
**key findings**<br>
-From the 6 month dataset the month June has the max toal rides each day of the week.
-the customer(casual riders) summary table showed that they tend to ride through the shoreline where their are leisure activity that is used  relax and enjoy yourself.
the Annual subscriber ride the bicycles more in the inner part of cities than the customers(casual rider).
-There are common bike stations where both subscribers and casual riders start from, and it is in high volume .<br><br>

## Map layout of how many customer started from the station, customer(casual riders) count above500 for the months of Jan,feb,mar <br>

![map q1](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/b6fd2b15-9fda-4e2e-8048-8cd11925d4da) <br>
To view the Tableau map layout Vizualization <a href="https://public.tableau.com/app/profile/nebyou.daniel/viz/howmanycustomerstartedfromstartstateionabove500q1/Sheet1?publish=yes">click here</a>

## Map layout of how many customer started from the station, customer count(casual riders) above 3000 for the months of apr,may,june

![map q2](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/fd00c818-18da-4872-8a93-78c2989b5bcb) <br>
To view the Tableau map layout Vizualization <a href="https://public.tableau.com/app/profile/nebyou.daniel/viz/customeronstartlocationabove3000/Sheet1?publish=yes">click here</a>

## Map layout of how many customer started from the station, subscriber count(annual member) above 2300 for the months of jan,feb,mar

![subscriber q1](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/29c8520a-3340-43ea-a16c-fa84851d07c4)<br>

To view the Tableau map layout Vizualization<a href="https://public.tableau.com/app/profile/nebyou.daniel/viz/howmanysubscribersstartedfromthatstationabove2300countformonthofjanfebmar/Sheet1?publish=yes">click here</a>
## Map layout of how many customers started from the stations , subscriber count(annual member) above 3500 for the months of apr,may,june 

![subscriber q2](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/ca5944ed-a3c4-4b6e-9da4-885cb4b515d0) <br>
To view the Tableau map layout Vizualization<a href="https://public.tableau.com/app/profile/nebyou.daniel/viz/howmanycustomersstartfromthatstationcountabove3500formonthofaprilmayjune/Sheet1?publish=yes">click here</a>



![total rides of customer each month](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/85b3cdaf-508e-456e-9369-90860e68fdfb)

![Total Rides(Minutes) in each day of the six month](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/87275f38-ce7f-4f38-bfe7-cfca87c858d7)

![Total rides(Minutes) of Subscribers each month](https://github.com/NEB73/capstone-case-study-cyclystic/assets/151795453/c015a5d8-899d-4ef6-80da-39b6df12cc36)


**Phase - 6 Act**

**Top Three Recommendations** <br><br>
1.Is to target the month of june to advertize and execute marketing campaign since that is the most interactive and high usage month for customers <br><br>
2.Target the the shoreline locations more since that where most of the customer use the bikes locations like,Adler Planetarium,Buckingham Fountain
,Burnham Harbor,Dusable HarborField Museum,Lake Shore Dr & Monroe St,Lake Shore Dr & North Blvd,McClurg Ct & Illinois St,Michigan Ave & Oak St,Millennium Park,Montrose HarborShedd Aquarium,Streeter Dr & Grand Ave,Theater on the Lake <br><br>
3.To create a a month sample plan to test out for a lower price so that customers can see the use of subscription by adding a subscribers bike section in each station where some of the bike can only be accessed by subscribers.<br><br>

