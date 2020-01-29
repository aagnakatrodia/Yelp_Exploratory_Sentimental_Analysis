<h1>Yelp Dataset Analysis - Exploratory</h1>

In the first part of this project, I will be performing all the exploratory analysis on the Yelp dataset. There are visualizations on the analysis of the data as well as various maps to show the distribution of reviews/checkins across the continents. It is further analyzed into the sections where the review count is maximum (Las Vegas, Nevada)

Dataset

This project uses the Yelp Open Dataset:https://www.yelp.com/dataset/download, which includes 5 files:

business: Contains business data including location data, attributes, and categories.<br><br>
review: Contains full review text data including the user_id that wrote the review and the business_id the review is written for.<br><br>
user: User data including the user's friend mapping and all the metadata associated with the user.<br><br>
checkin: Checkins on a business.<br><br>
tip: Tips written by a user on a business. Tips are shorter than reviews and tend to convey quick suggestions.<br>

For the purpose of my exploratory analysis, I am using the business, review, checkin dataset.

<b>Things done:</b>


•	Plot for distribution of Reviews across stars (1,2,3,4,5)<br><br>
![](Images/Exploratory/Stars.png)
•	Plot to show maximum category business. As, we can see, the maximum category of business is Restaurant, followed by Food and Shopping.<br><br>
•	World map to show where the restaurant businesses are scattered. I am using Basemap here with the 'hammer' projection to display the map. The background of the map is filled by etopo(). The red spots are the restaurant businesses included in the Business Dataset.<br><br>
•	Closer view of North America and Europe map for restaurant businesses. Again, I am using Basemap with bluemarble() for the background. The yellow spots are the restaurant businesses in the North America And Europe region<br><br>
•	Plot for Businesses with maximum Checkin counts<br><br>
•	Plot for Businesses with maximum Review counts<br><br>
•	Pie Chart of States with the maximum number of Checkins<br><br>
•	Map - Arcgisimage of Nevada. As we can see from the above pie chard, Nevada has the maximum number of checkins. In the below map, I am analyzing the Nevada region in further detail. I am using arcgisimage with the service 'NatGeo_World_Map' to show the Nevada region. As we can see, most of the restaurant businesses are concentrated across the Las Vegas region.<br><br>
•	Map - with inset function for Nevada. For this map, I am using the mark_inset function to give us a view of Las Vegas in a separate map inside the previous one<br><br>
•	Folium Map - With Headmap over time for review counts for Las Vegas. I am creating a heatmap over the time for the review_counts in the business/restaurant dataset by subsetting the location for Las Vegas. I will be using Folium Map with the plugin HeatMapWithTime<br><br>
•	States having average star ratings greater than 3 and less than 3. This results in a diverging plot<br><br>

