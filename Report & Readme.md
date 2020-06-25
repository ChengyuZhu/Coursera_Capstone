# Coursera_Capstone

#### Hi, there is a python project focusing on data science. I am still working on it.
#### BTW, I don't know how to trust the notebook to show the map I created. Anyone knows how to solve it? Thanks in advance! :)

### 1 Introduction
#### In this project, I will focusing on finding the similarities of neighbours among Downtown Toronto, Downtown New York City, and Downtown Beijing. Although the culture, the location, and the economic status may influence the similarities of those three cities, I want to drive some insights about common points from my analysis. Then, I will give some recommendation about which kind of interests or neighbours are popular among those big cities around the world based on the analysis. 

#### 1.1 Backgroud
#### Nowadays, the globalization is developing rapidly. Beijing, Toronto, and NY City are top biggest cities around the world. Beijing is located far from Toronto and NY city, and it's a city with different culture and economic status compared with Toronto and NYC. Toronto and NYC are much similar, but there is still different since the policy, the people and the season are quite different from each other. Beijing, Toronto, and NYC are representative cities of Asia and North America.
#### 1.2 Business Problem 
#### There are lots of companies which want to start their global business. However, the markets around the world are similar and dissimilar in the meantime. Thus, to understand which kind of business or whether to open the stores in a particular city is very important for every company which decide to focus on the global market (especially among Asia and America). To analyze the similarities of Beijing, Toronto, and NYC (as the representatives of big cities) can help those companies to understand the different situations and decide which kind of business branch is worth investing.


### 2 Data description
#### The data will be downloaded from the Internet (including wikipedia and json files and csv files downloaded from open data source). The datasets will contain the boroughs, neighbourhoods, coordinates (latitudes and longtitudes) information of Toronto, New York City, and Beijing. 
#### 2.1 Data Dictionary
⋅⋅* Boroughs: I will only keep boroughs related to downtown parts of those three cities.
⋅⋅* Neighbourhoods: neighbourhoods will be used to create clusters.
⋅⋅* Coordinates: Coordinates including data of latitudes and longtitudes, which will be used to plot maps.
⋅⋅* Venue: The venues around the certain neighbourhoods.
⋅⋅* Venue Type: the types of venues which got from Foursquare.
#### 2.2 Data Cleaning
#### Since I want the information about the downtown in those three cities, we just select the data recorded the downtown district.
#### There are some missing values of Toronto dataset, and the missing values are deleted.
#### After importing the location data of Beijing dataset, there are 6 neighbourhoods which don't have their location informaton. However, there are still 35 avaiable values, so we still think the dataset is enough to be analyzed.

### 3 Methodology

#### 3.1 Clustering
#### After getting the cleaned data, I wanted to analyze the venue types. Then I created the map of each cities and then using the mean to get the 3 most common venues of each neighbourhoods in the downtown district. Then I clustered the venue types of each cities.
#### 3.2 Explanation Analysis
#### To get the top 3 venues of the neighbours at downtown area, I aggregated the number of each venue and then understood the most popular venues of each city:
..* Toronto: Coffee shop, cafe, and Park
..* New York: Coffee shop, Italian restaurant, cafe
..* Beijing: Chinese restaurant, Hotel, Fast food restaurant
#### It can be found that Toronto and New York are more similar. However, the numbers of coffee shop and cafe are also large.
#### To get the common venues of three cities, venn diagram was plotted. There are 6 venues_types are in those three cities: Bakery, Bar, Cafe, Coffee shop, hotel, and park.
#### NYC and Toronto has 8 coomon venues types, NYC and Beijing have 5 common venues types, and Toronto and Beijing have only 1 common venues. 
#### To get the unique venues of each cities, union function is used. There are 55 unique venues. Among them, fast food restaurant, Gym, and American restaurant have great amount compared with other types.

### 4 Results
#### From the analysis, it can be found that Beijing is quite different from Toronto and NYC. Toronto is more similar with NYC, but it has less special venues compared with other two cities. NYC is both similar to Beijing and Toronto, and it also has its own features. Beijing is quite unique since it has different culture. 
#### However, there are also common venues types, which are Bakery, Bar, Cafe, Coffee shop, hotel, and park. Among those types, bakery, bar, cafe and coffee shop are related, and they are all related to food and eating. Thus, if a company wanted to open their global busines or open a new brand in a different city, catering or relative business is a great idea. The company also needs pay attention to the categories of restaurant beacause of the different tastes of food. Coffee shop or cafe is a global choice.

### 5 Discussion
#### In this project, I only used three cities as the representatives, so there is still limitation. Fortunately, the cities are located far from each other, so we can think the result is useful to some extend. If there are more cities are considered, the results may be slight different.
#### The types of restaurants are quite different, and i considered them as different types. If we consider them as a common type, the results maybe different. We can still foresee that catering is the most popular choice from the current analysis, but more choices can be found.

### 6 Conclusion
#### In this project, I used the location data to build maps and clustered the venues types of three cities: Beijing, New York City, and Toronto. For a company or entrepreneur that wants to open a new brand or start new business globally, opening a catering-related brand at downtown is a best choice. However, the local taste should be considered. Besides, coffee shop and cafe are popular around the world.
