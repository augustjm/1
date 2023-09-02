 ### How does weather conditions in Singapore affect Mosquito borne diseases in Singapore.

 - Preliminary findings shows that Mosquitoes thrive in warm and humid conditions. 

 - Due to the nature of the data gathered, the analysis will be focused on Geopraphical data which shows the following:
          (1): Rainfall intensity as of July 2023
          (2): Mean temperature as of July 2023
          (3): Streamlit data(app.py) located in "code folder" which shows the current Cluster of Singapore
               as of August 2023

 - Files used to compile data stored in the notebook:
          (1): rainfall-monthly-highest-daily-total
          (2): rainfall-montnly-number-of-rain-days
          (3): rainfall-monthly-total
          (4): dengue_cases
 
 - Files used to generate streamlit geo-map
          (1): DengueClustersGEOJSON.geojson
          (2): DengueClusterKML.kml

 - Files cleaned and subsequently merged:
          (1): cleaned_merged_rainfall
          (2): cleaned_dengue_cases


### Problem statement: How to properly managge and predict dengue outbreaks:

This README aims to dispel myths and provide insights into the relationship between weather conditions and the prevalence of dengue fever in Singapore. While many Singaporeans believe that rainy days cause dengue, it's important to understand that they actually create an environment conducive for Aedes mosquitoes, the vectors responsible for transmitting the dengue virus.

Common Misconception:
In the tropical climate of Singapore, the assumption is often made that rainy days are the cause of dengue outbreaks.

The Fact:
Rainy days themselves do not cause dengue fever. However, they do provide ideal breeding conditions for Aedes mosquitoes. Stagnant water resulting from frequent rain showers can accumulate in places like flower pots, discarded containers, and even gutters, serving as breeding grounds for these mosquitoes.


Warm and Humid Climate: A Catalyst for Dengue:
Singapore's warm and humid climate speeds up the life cycle of the Aedes mosquito and allows for quicker replication of the dengue virus within the mosquito. This increases the mosquito's infectivity, thereby raising the risk of dengue transmission.


Data dictionary:

Rainfall data (`cleaned_merged_rainfall.csv`)

| Feature              | Type        | Dataset       | Description                                                |
|---------------------|-------------|---------------|------------------------------------------------------------|
| `month`              | datetime64  | Rainfall Data | The month and year of the recorded data                     |
| `year`               | integer     | Rainfall Data | The year of the recorded data                               |
| `month_only`         | integer     | Rainfall Data | The month (1-12) of the recorded data                       |
| `max_rainfall_in_a_day` | float64  | Rainfall Data | Maximum rainfall in a single day (in mm)                    |
| `num_rainy_days`     | float64     | Rainfall Data | Number of days in the month with rainfall                   |
| `total_rainfall`     | float64     | Rainfall Data | Total amount of rainfall in the month (in mm)               |




Dengue cases data (`cleaned_dengue_cases.csv`)

| Feature         | Type    | Dataset         | Description                                 |
|-----------------|---------|-----------------|---------------------------------------------|
| `year`          | integer | Dengue Cases Data | The year of the recorded data               |
| `dengue_fever`  | integer | Dengue Cases Data | Number of recorded cases of Dengue Fever    |


Conclusion:
Both rainy days and the warm, humid climate of Singapore contribute to conditions favorable for the Aedes mosquito but are not direct causes of dengue fever. By taking appropriate preventative measures, the risk of dengue can be minimized.

Recommendations:

A predictive model can be formed with more in-depth data made available by the following agencies (National Environment Agency, Meteorological Service Singapore).





