## **Project Aims and Background**
A laundry-pickup sevices startup is in a Blue Ocean that are building its network in smaller citites that are not targeted by the big players in the laundry service industry. This startup already had a strong presence in 140 locations in the USA. It has recently opened stores in 10 new cities. The company would like to find out which of the 10 new locations have the best potential for the company to invest more funds into marketing and can potentially have the best ROMI (Return on marketing investment).

## **Exploratory Data Analysis via Data Visualization**
First we want to get a good idea of where the services are located in the United States. And we can also visualize how much revenue the cities are roughly earning, the bigger the circles, the more the revenue.

![Image](https://raw.githubusercontent.com/claire-cheng/Laundry-Pickup-Marketing-Strategy/master/Service%20locations.png).

We can see from the image that the services location of the startup are spreaded throughout the country. But it is not visible to us whether there is a trend in the revenue or not just by looking at this map.

Since this project is focusing on the services in the new cities, we want to highlight those new cities to see where they are located in the map.

![Image](https://raw.githubusercontent.com/claire-cheng/Laundry-Pickup-Marketing-Strategy/master/New%20cities%20locations.png).

We can see from the graph that the new cities are located in California, Arizona, Texas, Illinois, Tennessee, and New Jersey. And it seems like other than that one city in Texas, all the other cities are earning relatively similiar amount of revenue.
New that we know where the new cities are located, we can dig deeper with analytics to see if there are any trends that can help us draw some insights and make meaningful decisions for this laundry-pickup service startup.

## **Cluster Analysis**
ROMI is calculated based on revenue and marketing investment, so we want to see how the distribution and relationship looks like between these two variables for each city. 

![Image](https://raw.githubusercontent.com/claire-cheng/Laundry-Pickup-Marketing-Strategy/master/Clustering%20without%20population.png).

Just by eyeballing the visualization, it seems like our data can be grouped into two clusters based on the revenue, one roughly above 30K and the other cluster lies below 30K. However, Tableau decided to group the two clusters a little bit different than what we expected. As shown in the graph above, Tableau seperated the two clusters by 36K instead of the 30K we anticipated in the beginning. Due to the differences, we would want to look into the graph more closer to see if there are any trends identified for each cluster. As we can see from Cluster 1, there seems to be a positive linear trend that indicates the higher the marketing spend, the higher the return on ROMI- the revunue returned from the services provided at a specific city. The behavior in Cluster 1 is anticipated as ideally, the more we invest in something, the more ROI we would expect to be returned. Whereas for Cluster 2, it seems that there is also a trend here with a linear trend with a slope that is close to 0. This indicates that for those cities that are in this cluster, it does not matter how much money we are spending on marketing, the revenue that is generated from these cities are not increasing as the expected behavior. As a result of this initial cluster analysis, it makes us wonder if there is some other factors that are affecting these cities in Cluster 2. 
Population plays a big role in launry services, as the more people there are in a city, the more dirty laundry there are that would be needing laundry services. What if the population size in the cities in Cluster 2 are relatively small, so that no matter how much money we spend on marketing would not add value to increasing number of laundry services needed, let alone generating more revenue. In this case, we are going to use external data sources to provide us the size of the population of the cities the startup has its services in. 

![Image](https://raw.githubusercontent.com/claire-cheng/Laundry-Pickup-Marketing-Strategy/master/Clustering%20with%20population.png).

As shown in the graph above, we are including our external data on the population in the cities into our original dataset and using Tableau to recluster the new dataset. Tableau has grouped our data into three clusters and we drew linear trend lines across that data points in each cluster to make the graph even easier to be visualized. Tableau seperated the clusters by grouping the cities with closer population sizes into the same cluster. Cluster 3 (Red) has a population size of 150K and above, Cluster 1 (Blue) has a population size between 120K and 150K, and Cluster 2's population size (Orange) lies below 120K.

(talk about the lower group where revenue is not increasing when marketing spend is increasing. the first group seems to be alright. maybe this is why tableau group them differently because something else is up. this is why we use external data- population to regroup the clusters to see if it would give us a different result).
