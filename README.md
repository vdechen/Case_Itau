# Case_Itau
 
# Project Goal and Description
  The goal of this project was to create a model to predict whether it might rain in Australia tomorrow, according to hystorical data. 
  
# Technologies 
  - Python (Pandas, Numpy, Seaborn, SkLearn, Statsmodels)
  - Tableau

# Steps
- Exploratory analysis was made in the 'rain' dataset, which initially contained 142193 rows. 
- The 'rain' dataset was normalized.
- 'raintoday' and 'raintomorrow' variables were dummified. 
- Strong correlations were identified between 'raintomorrow' and sunshine(-0.450768), cloud3pm (0.381870), humidity3pm (0.446160) and humidity (0.405600) variables. However, some of these contained a lot of nulls (67816, 57094, 3610 and 3610, respectively).
- Even stroger correlations were noticed between 'raintomorrow', 'amountOfRain'(0.501485) and 'modelo_vigente'(0.825086), so these last columns were dropped due to data leakage. 
- 'humidity3pm' (3610) and 'rainfall' (1297) nulls were dropped, so these variables could also be used in modeling.
- Different trial models were created. 
- The best performance was obtained for 4 different location groups separated by average humidity. The interval average humidity interval for each group was (0) = [-1.213, -0.706], (1) = [-0.706, -0.201], (2) = [-0.201, 0.303] and (3) = [0.303, 0.808]. Train and test accuracy scores were, respectively (0.93, 0.93), (0.86, 0.86), (0.83, 0.82), (0.78, 0.78). 

# Conclusion

   
# Contact
- LinkedIn: vanessadechen
- GitHub: /vdechen
- Email: vanessadechen@gmail.com
