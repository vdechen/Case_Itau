# Case_Itau
 
# Project Goal and Description
  The goal of this project was to create a model to predict whether it might rain in Australia tomorrow, according to hystorical data. This is an Itaú Bank case study from  a hiring process for a data scientist role. 
  
# Technologies 
  - Python (Pandas, Numpy, Seaborn, SkLearn, Statsmodels)
  - Tableau

# Steps
- Exploratory analysis was made in the 'rain' dataset, which initially contained 142193 rows. 
- The 'rain' dataset was normalized; 'raintoday' and 'raintomorrow' variables were dummified. 
- Strong correlations were identified between 'raintomorrow' and sunshine(-0.450768), cloud3pm (0.381870), humidity3pm (0.446160) and humidity (0.405600) variables. However, some of these included a lot of nulls (67816, 57094, 3610 and 3610).
- Even stroger correlations were noticed between 'raintomorrow', 'amountOfRain'(0.501485) and 'modelo_vigente'(0.825086), so these last columns were dropped due to data leakage. 
- 'humidity3pm' (3610) and 'rainfall' (1297) nulls were dropped, so these variables could also be used in modeling.
- Different trial models were created and accuracy scores were checked for performance evaluation. 
- An exploratory data analysis of the 'wind' dataset was initiated after renaming columns and merging them with the 'rain' datatset. Higher averages for wind speed at 9am and 3pm can be noticed in Tableau graphics the day before it rains, but further analysis is to be continued. 

# Conclusion

Australia climate is highly influentiated by a big desert in the middle of the country and the coastline surrounding it, which creates different humidity areas that needed to be taken into account for rain prediction modeling. Therefore, the best performance was obtained in Logarithmic Regressions for 4 different groups using 'humidity3pm', 'humidity','raintoday', 'temp3pm' and 'rainfall' variables, separated by location and average humidity. The average humidity interval for each group was (0) = [-1.213, -0.706], (1) = [-0.706, -0.201], (2) = [-0.201, 0.303] and (3) = [0.303, 0.808]. Train and test accuracy scores were (0.93, 0.93), (0.86, 0.86), (0.83, 0.82) and (0.78, 0.78), respectively. The model still needs improvement on predicting positive rain days, so explorationg of correlations between rain and wind variables are recommended for further development. 
 
# Contact
- LinkedIn: vanessadechen
- GitHub: /vdechen
- Email: vanessadechen@gmail.com
