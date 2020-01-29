# Capstone

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

Cluster 0: Neighborhoods with little or no Middle Eastern restaurants
Cluster 1: Neighborhoods with no Middle Eastern restaurants
Cluster 2: Neighborhoods with high number of Middle Eastern restaurants
The results are visualized in the above map with Cluster 0 in red color, Cluster 1 in purple color and Cluster 2 in light green color.

## Recommendations

Most of Thai restaurants are in Cluster 2 which is around Adelaide, King, Richmond areas and lowest (close to zero) in Cluster 1 areas which are North Toronto West and Parkdale areas. Also, there are good opportunities to open near Chinatown, St James town as the competition seems to be low. Looking at nearby venues, it seems Cluster 1 might be a good location as there are not a lot of Asian restaurants in these areas. Therefore, this project recommends the entrepreneur to open an authentic Burmese restaurant in these locations with little to no competition. Nonetheless, if the food is authentic, affordable and good taste, I am confident that it will have great following everywhere =)

Limitations and Suggestions for Future Research

In this project, I only take into consideration of one factor: the occurrence / existence of Thai restaurants in each neighborhood. There are many factors that can be taken into consideration such as population density, income of residents, rent that could influence the decision to open a new restaurant. However, to put all these data into this project is not possible to do within a short time frame for this capstone project. Future research can take into consideration of these factors. In addition, I am relying on the existence of Thai restaurants only for this project but future research can take into consideration of other variables such as existence of Asian restaurants, Asian population level in each neighborhood etc.

Conclusion

In this project, we have gone through the process of identifying the business problem, specifying the data required, extracting and preparing the data, performing the machine learning by utilizing k-means clustering and providing recommendation to the stakeholder.
