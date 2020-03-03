## **Project Aims and Background**
A laundry-pickup sevices startup is in a Blue Ocean that are building its network in smaller citites that are not targeted by the big players in the laundry service industry. This startup already had a strong presence in 140 locations in the USA. It has recently opened stores in 10 new cities. The company would like to find out which of the 10 new locations have the best potential for the company to invest more funds into marketing and can potentially have the best ROMI (Return on marketing investment).

## **Exploratory Data Analysis via Data Visualization**
First we want to get a good idea of where the services are located in the United States. And we can also visualize how much revenue the cities are roughly earning, the bigger the circles, the more the revenue.

![Image](https://github.com/claire-cheng/Laundry-Pickup-Marketing-Strategy/blob/master/Service%20locations.png).

We can see from the image that the services location of the startup are spreaded throughout the country. But it is not visible to us whether there is a trend in the revenue or not just by looking at this map.

Since this project is focusing on the services in the new cities, we want to highlight those new cities to see where they are located in the map.

![Image](https://github.com/claire-cheng/Laundry-Pickup-Marketing-Strategy/blob/master/New%20cities%20locations.png).

We can see from the graph that the new cities are located in California, Arizona, Texas, Illinois, Tennessee, and New Jersey. And it seems like other than that one city in Texas, all the other cities are earning relatively similiar amount of revenue.
New that we know where the new cities are located, we can dig deeper with analytics to see if there are any trends that can help us draw some insights and make meaningful decisions for this laundry-pickup service startup.

## **Cluster Analysis**
ROMI is calculated based on revenue and marketing investment, so we want to see how the distribution and relationship looks like between these two variables for each city. 

![Image](https://raw.githubusercontent.com/claire-cheng/Laundry-Pickup-Marketing-Strategy/master/Clustering%20without%20population.png).

Just by eyeballing the visualization, it seems like our data can be grouped into two clusters based on the revenue, one roughly above 30K and the other cluster lies below 30K. However, Tableau decided to group the two clusters a little bit different than we expected. As shown in the graph above, Tableau seperated the two clusters by 36K instead of the 30K we anticipated in the beginning.
(talk about the lower group where revenue is not increasing when marketing spend is increasing. the first group seems to be alright. maybe this is why tableau group them differently because something else is up. this is why we use external data- population to regroup the clusters to see if it would give us a different result).
