# Ticket amount prediction - Parking Tickets in Toronto

### Project Overview
---
Parking tickets across the city generate millions in revenue for the City of Toronto every year. Even though the City of Toronto's revenue from parking tickets has gone up slightly in the last 2-3 years, after Covid-19, it has been declining since 2019. There is an opportunity to reverse this decline by making the City of Toronto's Administrative Penalty System (APS) more efficient. Using machine learning can enhance the efficiency of the APS.The impact of an efficient model can make the city safer and more attractive to residents and tourists. 

- **Problem Area and Users**: The repercussions of an inefficient system extend beyond revenue loss. It also compromises the safety of the city's residents. Therefore, apart from the economic benefits for the city, this model would contribute to a safer Toronto for its residents.

- **Proposed Solution**: Leveraging machine learning can significantly enhance the effectiveness of the APS. The model will predict set fine amounts.

- **Impact**: The impact of such an efficient model would not only make the city safer but also attract more residents and tourists. The potential revenue increase could be as high as $30 million per year. 

- **Dataset Description**: Dataset description is moved to Data folder.

### EDA and Data Preprocessing
---

Inspected infraction_description values and removed redundant rows.

Inspected time_of_infraction, converted to datetime for EDA and later to int to use in the analysis.

Splitted date_of_infraction into day, month and year to use it in further analysis.

Used geolocator API to convert addresses to Latitude and Longitude. Converted location2 column, got 2500 unique rows.

Created classes of set_fine_amount tickets to fit Classification model.


### Baseline Models
---
-Logistic Regression

-Random Forest

-AdaBoost

-XGBoost

### Advanced Model

-XGBoost performed better than other models with 90 percent accuracy score. The model is not biased toward any specific class, demonstrating generalization across all classes.

### Next Steps
- Convert all addresses to Latitude and Longitude.

---

### References and Sources
---

- [Open Data Toronto](https://open.toronto.ca/dataset/parking-tickets/): dataset source

