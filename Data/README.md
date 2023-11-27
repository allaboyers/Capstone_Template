# Ticket Amount Prediction - Parking Tickets in Toronto

### Project Overview
---
Parking tickets across the city generate millions in revenue for the City of Toronto every year. Even though the City of Toronto's revenue from parking tickets has gone up slightly in the last 2-3 years, after Covid-19, it has been declining since 2019. There is an opportunity to reverse this decline by making the City of Toronto's Administrative Penalty System (APS) more efficient. Using machine learning can enhance the efficiency of the APS.The impact of an efficient model can make the city safer and more attractive to residents and tourists.




- **Dataset Description**: To implement this project, the data is sourced from the Open Data Portal of the City of Toronto (2020-2022). The dataset contains non-identifiable information regarding each parking ticket issued annually. These tickets are issued by personnel from Toronto Police Services (TPS) and authorized individuals. 

| ITEM   NAME            | DESCRIPTION                                                  |
|------------------------|--------------------------------------------------------------|
|                        |                                                              |
| TAG_NUMBER_MASKED      | First three (3) characters masked   with asterisks           |
| DATE_OF_INFRACTION     | Date the infraction   occurred in YYYYMMDD format            |
| INFRACTION_CODE        | Applicable Infraction   code (numeric)                       |
| INFRACTION_DESCRIPTION | Short description of   the infraction                        |
| SET_FINE_AMOUNT        | Amount of set fine   applicable (in dollars)                 |
| TIME_OF_INFRACTION     | Time the infraction   occurred  in HHMM format (24-hr clock) |
| LOCATION1              | Code to denote   proximity (see table below)                 |
| LOCATION2              | Street address                                               |
| LOCATION3              | Code to denote   proximity (optional)                        |
| LOCATION4              | Street address   (optional)                                  |
| PROVINCE               | Province or state   code of vehicle licence plate            |
|                        |                                                              |
|                        |                                                              |
| Proximity Code Table   |                                                              |
| PROXIMITY CODE         | DESCRIPTION                                                  |
| AT                     | At                                                           |
| NR                     | Near                                                         |
| OPP                    | Opposite                                                     |
| R/O                    | Rear   of                                                    |
| N/S                    | North   Side                                                 |
| S/S                    | South   Side                                                 |
| E/S                    | East   Side                                                  |
| W/S                    | West   Side                                                  |
| N/O                    | North   of                                                   |
| S/O                    | South   of                                                   |
| E/O                    | East   of                                                    |
| W/O                    | West   of                                                    |

 

#
- The dataset can be downloaded from the following website.
- [Open Data Toronto](https://open.toronto.ca/dataset/parking-tickets/): dataset source
- Converted addresses to latitude and longitude can be found in this folder.
