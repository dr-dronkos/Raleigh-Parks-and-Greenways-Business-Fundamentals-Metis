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

## Tools and Methodology
Google Sheets was used to clean and perform preliminary exploratory data analysis of each data set. Google Sheets was also used to group the 42 activities available at the parks into 7 larger categories to be used as filters in Tableau.  Python was used to pair Location ID columns in the Raleigh Greenway Trails dataset with .geojson files also available from Open Data Raleigh to recover latitude and longitude coordinates. Python was also used to pair these coordinates with the ZIP code data to make the datapoints searchable by ZIP code in the interactive dashboard. The dashboard was created using Tableau Public, and allows users to filter both parks and greenways by ZIP code. Greenway data can additionally be filtered by Accessibility and Length (Long trails are longer than 5 miles; Short trails are shorter than 3 miles). Park data can be filtered by Arts (contains an arts center, museum, library, etc.), Bike or Skate (contains bike trails, a skate park, a BMX track, etc.), Family (contains a community center, playground, picnic tables, etc.), Fitness (contains a gym, fitness course, track, etc.), Pets (allows dogs or horses), Sports (contains baseball fields, tennis courts, handball courts, etc.), and Watersports (allows boating, fishing, or canoeing, etc.).

## Business Context
The client here is the Wake County Open Space and Parks Advisory Committee and the City of Raleigh, who administer the parks and greenways system addressed in this project. This project hypothesizes that giving people access to searchable information about the parks and greenways in a single dashboard will boost their engagement with the parks and geenways system, and also improve the public's opinion of the parks and greenways system.

Some possible critera for success:
-	Ten percent of the population of Wake County, so around 110,000 people, use the recommendation dashboard 
-	The Committee is able to use the collected data to show the Board of Commissioners that they are fulfilling their mission, and to negotiate for increased funding

Assumptions:
-	Community members will use the interactive dashboard
- Community members have internet access

Risks:
- No one will use the pilot dashboard and it will be a waste of time and money
- Presenting the aggregated data to the Board of Commissioners will result in a reduction in funding
- The interacrtive dashboard will perform poorly and as a result the community will have a more negative opinion about the parks/greenways and the Committee

## Future Work
After the interactive dashboard is presented to the Wake County Open Space and Parks Advisory Committee and piloted in the community, interative improvements will be made. If public response is positive and people seem to be using the dashboard, steps can be taken to develop a data pipeline to start collecing data from users as they interact with the dashboard. This data can then be used to create a prescriptive machine learning model that will power a Parks and Greenways Recommender. This platform can be augemented over time based on user feedback and as more data is collected. Eventually, insights this data can be used to inform future park and greenway expansion projects.

## Communication
[Business_Fundamentals_Metis_Danielle_Ronkos.pdf](https://github.com/dr-dronkos/Raleigh-Parks-and-Greenways-Business-Fundamentals-Metis/files/8329543/Business_Fundamentals_Metis_Danielle_Ronkos.pdf)

