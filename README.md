# Optimal Location for Opening a Middle Eastern Restaurant

## Introduction

Toronto: Ontario’s most cosmopolitan city, which is often referred to as ‘the most multicultural city in the world, with around half of its population born outside the country. With international neighbourhoods and thriving foodservice landscape, Toronto is a hub for great international restaurants from all around the world, especially the Middle East. Although a quick search on the internet shows that there are not enough Middle Eastern Restaurants in the city. The aim of this project is to explore the idea of opening a Middle Estern restaurant in the city and finding the most suitable location for it, taking into account the demographic of the neighbourhoods and the locations with popular Middle-Eastern restaurants, by using machine learning methods such as clustering.

## Data

List of neighborhoods in Toronto, Canada.
Latitude and Longitude of these neighborhoods.
Venue data related to Middle Eastern restaurants. 

## Methodology

I got the list of neighborhoods in Toronto, Canada from wikipedia page (“https://en.wikipedia.org/wiki/List_of_postal_codes_of_Canada:_M”)

I got the coordinates using the csv file provided by IBM team. In the next step, I used Foursquare API to get the list of top 100 venues within 500 meters radius. Then, I analyze each neighborhood by grouping the rows by neighborhood and taking the mean on the frequency of occurrence of each venue category, to prepare clustering to be done later.

Then I performed the clustering method by using k-means clustering.I have clustered the neighborhoods in Toronto into 3 clusters based on their frequency of occurrence for “”. 
Results

### Clusters

Based on the results (the concentration of clusters), I will be able to recommend the ideal location to open the restaurant.

The results from k-means clustering show that we can categorize Toronto neighborhoods into 3 clusters based on how many Thai restaurants are in each neighborhood:
map_clusters.save('map_clusters.html')
Cluster 0: Neighborhoods with little or no Middle Eastern restaurants
Cluster 1: Neighborhoods with no Middle Eastern restaurants
Cluster 2: Neighborhoods with high number of Middle Eastern restaurants
The results are visualized in the above map with Cluster 0 in red color, Cluster 1 in purple color and Cluster 2 in light green color.

## Recommendations

Most of Mimddle Eatern restaurants are in Cluster 2 which is around Dovercourt Village, and lowest (close to zero) in Cluster.It seems Cluster 1 might be a good location as there is only one Middle Eastern restaurants.
