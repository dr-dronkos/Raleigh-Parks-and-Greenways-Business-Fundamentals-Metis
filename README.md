# Raleigh-Parks-and-Greenways-Business-Fundamentals-Metis

# Raleigh Parks and Greenways Recommender

## Abstract
This project uses data from Open Data Raleigh (https://data-ral.opendata.arcgis.com/) to create an interactive dashboard allowing users to find parks and geenways in the greater Raleigh area by location, features, and amenities. The created dashboard functions as a Minimum Viable Product on the path to eventually developing a prescriptive machine learning model to recommend new parks and greenways to users based on their previous activity and interests. An additional goal of the project is to collect user data, following ethical best practices, that can be used by the Wake County Open Space and Parks Advisory Committee to inform future expansion of the parks and greenways system.

## Data
The project used three open source data sets available on Open Data Raleigh:
- Parks in Wake County (290 rows)
(https://data-ral.opendata.arcgis.com/datasets/Wake::parks-in-wake-county/explore)

- Raleigh Greenway Trails (1249 rows)
(https://data-ral.opendata.arcgis.com/datasets/ral::raleigh-greenway-trails/explore?location=35.818950%2C-78.627250%2C11.53)

- ZIP Code Boundaries in Wake County
(https://data-ral.opendata.arcgis.com/datasets/Wake::zip-codes/explore?location=35.798550%2C-78.619900%2C10.58)
![image](https://user-images.githubusercontent.com/95940978/159618572-0a01c66b-916a-44a8-9f94-88bb22a80fba.png)

## Tools and Methodology
Google Sheets was used to clean an perform a preliminary exploratory data analysis of each data set. Google Sheets was also used to group the 42 activities available at the parks into 7 larger categories to be used as filters in Tableau.  Python was used to pair Location ID columns in the Raleigh Greenway Trails dataset with .geojson files also available from Open Data Raleigh to recover latitude and longitude coordinates. Python was also used to pair these coordinates with the ZIP code data to make the datapoints searchable by ZIP code in the interactive dashboard. The dashboard was created using Tableau Public, and allows users to filter both parks and greenways by ZIP code. Greenway data can additionally be filtered by Accessibility and Length (Long trails are longer than 5 miles; Short trails are shorter than 3 miles). Park data can be filtered by Arts (contains an arts center, museum, library, etc.), Bike or Skate (contains bike trails, a skate park, a BMX track, etc.), Family (contains a community center, playground, picnic tables, etc.), Fitness (contains a gym, fitness course, track, etc.), Pets (allows dogs or horses), Sports (contains baseball fields, tennis courts, handball courts, etc.), and Watersports (allows boating, fishing, or canoeing, etc.).

