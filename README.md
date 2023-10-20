# Revenue Forecasting - Parking Tickets in Toronto

### Project Overview
---
Parking tickets generate around $90 million in revenue for the City of Toronto's budget. However, the city's revenue from parking tickets is on the decline year after year. There is a significant opportunity to reverse this decline and even increase revenue by enhancing the efficiency of the City of Toronto's Administrative Penalty System (APS).

- **Problem Area and Users**: The repercussions of an inefficient system extend beyond revenue loss. It also compromises the safety of the city's residents. Therefore, apart from the economic benefits for the city, this model would contribute to a safer Toronto for its residents.
Parking enforcement officers can also reap rewards from this system, as it would enable them to meet their daily quotas and earn bonuses. The Toronto Board of Trade has pointed out that gridlock, caused by blocked traffic lanes, poses the most significant threat to economic prosperity, costing the region billions annually.


- **Proposed Solution**: Leveraging machine learning can significantly enhance the effectiveness of the APS. The model can identify priority areas with a high incidence of illegal parking, categorizing them based on recent infractions (e.g., last month or last week) and the highest fine amounts.


- **Impact**: The impact of such an efficient model would not only make the city safer but also attract more residents and tourists. The potential revenue increase could be as high as $30 million per year. Additionally, by mitigating gridlock issues, we can prevent potential economic losses estimated at $6 billion, as reported by the Toronto Board of Trade in 2011.


- **Dataset Description**: To implement this project, we will source data from the Open Data Portal of the City of Toronto (2020-2022). The dataset contains non-identifiable information regarding each parking ticket issued annually. These tickets are issued by personnel from Toronto Police Services (TPS) and authorized individuals. It's important to note that the dataset only includes complete records, and incomplete entries present minimal impact on trend analysis. Incompleteness might be due to reasons such as out-of-province vehicle registrations or tickets being paid before staff could enter them into the system.

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

 

### Next Steps
---
Inspect the location columns to determine whether some of them can be dropped or if they should be concatenated with other location columns.

Inspect location2 addresses to assess whether we can group them by proximity and reduce the number of distinct values

Inspect infraction_description values to assess whether we can group them by some similarity and reduce the number of distinct values

Inspect time_of_infraction, find the problem and convert it to Datetime data type

Concatenate date_of_infraction and time_of_infraction columns

Convert location to Latitude and Longitude

Statistics and relationships

### References and Sources
---

- [Open Data Toronto](https://open.toronto.ca/dataset/parking-tickets/): dataset source
- [Report: Administrative Penalty System – 2021 Activity](https://www.toronto.ca/legdocs/mmis/2022/gl/bgrd/backgroundfile-225640.pdf)
- [Article: TheStar](https://www.thestar.com/opinion/contributors/the-number-of-parking-tickets-has-plunged-in-cash-strapped-toronto-why-the-lax-enforcement/article_588cb2a7-843e-5e23-aef7-d8f2ff9afdb1.html#:~:text=The%20city's%20annual%20revenue%20from,estimated%20%2490%20million%20in%202021)
- [Article: CBC](https://www.cbc.ca/news/canada/toronto/parking-rules-don-t-apply-to-all-1.1045718)

