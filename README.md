# EDA Hotel Bookings

Hotel Bookings Analysis  
Analyzing Hotel Bookings and Cancellations  
By Mesum Raza Hemani [source]

**Repository Structure**  
```bash 
|___Data
|    |___hotel_bookings.csv #original data  
|    |___hotel_bookings_processed_data #cleaned data
|
|___Excels
|    |___hotel_bookings_raw_data #data cleaning
|    |___hotel_bookings_analysis #clean data
|____README

```



## About this dataset
The Hotel Bookings dataset is a comprehensive collection of information regarding hotel bookings, cancellations, and guests' details. This dataset provides insights into various aspects such as the type of hotel, the number of adults, children and babies per booking, the length of stay in both weekend nights (Saturday or Sunday) and weekdays (Monday to Friday), the meal plan chosen by guests, their country of origin and market segment designation.

Additionally, this dataset includes significant information about reservation status and its updates. It covers whether a booking was canceled or not, the lead time between booking date and arrival date, the week number and day of arrival date. It also indicates if a guest is a repeated visitor or a new customer.

The dataset contains information related to room assignments as well. It mentions both reserved room types (the type of room initially requested) as well as assigned room types (the room actually allocated). Furthermore, it reveals any changes made to bookings along with details about previous cancellations made by guests.

Other relevant factors in this dataset are deposit type for each booking; ID numbers for travel agencies used in making reservations; days spent on waiting lists before confirmation; customer classification such as transient or group; average daily rate calculated based on lodging transactions divided by total staying nights; required car parking spaces indicated by customers; the total count of special requests made by each guest.

The provided data can facilitate analysis on several levels: studying specific hotels within different periods (including year), understanding trends across months and weeks within those years to identify preferred seasons among guests from various countries represented in terms of proportions over other nations. An examination can be conducted for differences between adult-only bookings vs family-oriented ones considering associated variables like stayed weekend/week nights for conversations around how these two groups differ when it comes to selecting their staying patterns at hotels.

This expansive dataset has great potential for an in-depth exploration into various aspects involved in hotel bookings processes while providing valuable insights for improving hotel services, optimizing operations, and understanding customer preferences

## How to use the dataset

### Introduction:

Understanding the Columns:

**hotel:** Type of hotel (Categorical)

**is_canceled:** Whether the booking was canceled or not (Binary)

**lead_time:** Number of days between booking date and arrival date (Numeric)

**arrival_date_year**:** The year of the arrival date (Numeric)

**arrival_date_month:** The month of the arrival date (Categorical)

**arrival_date_week_number:** The week number of the arrival date (Numeric)

**arrival_date_day_of_month:** The day of the month of the arrival date (Numeric)

**stays_in_weekend_nights:** Number of weekend nights stayed or booked to stay at the hotel (Numeric)

**stays_in_week_nights:** Number of week nights stayed or booked to stay at the hotel (Numeric)

**adults, children, babies:** Number of guests categorized by age groups

adults = Number of adults  
children = Number of children  
babies = Number infants  


### **Booking Details:**

**-meal:** Type(s) food option(s) included in booking package (Categorical)  
**-country & market_segment & distribution_channel** columns provide demographic and customer classification information.  
**-is_repeated_guest** column specifies whether a guest is a repeated visitor or not.  
**-previous_cancellations** column indicates how many previous bookings were canceled by a guest.  
**-previous_bookings_not_canceled** shows how many previous bookings were not canceled by a guest.  

### **Accommodation Details:**

**-reserved_room_type** column indicates which type room was originally reserved for each booking.  
**-assigned_room_type** mentions which type room was finally assigned for each booking.  
**-booking_changes** Number of changes made to the booking before arrival.  
**-deposit_type** Type of deposit made for the booking (Categorical).  
**-agent & company** columns provide relevant information about the travel agency and/or company involved in making the reservation.  

### **Additional Information:**

**-days_in_waiting_list:** Number of days the booking was on a waiting list before it was confirmed or canceled.  
**-customer_type** provides information on types of customers (Categorical)  
**-adr:** Average daily rate per room, calculated by dividing the sum of all lodging transactions by the total number of staying nights (Numeric)


## Research Ideas  

***Demand Forecasting:***  The dataset can be used to analyze booking patterns and trends, such as the number of bookings made over time, the seasonality of bookings, and the impact of certain factors (e.g., lead time, arrival date) on booking behavior. This information can help hotels forecast future demand and optimize their pricing and inventory management strategies.  

***Customer Segmentation:*** By analyzing various attributes in the dataset such as market segment, customer type, and special requests made by guests, hotels can identify different customer segments with unique needs and preferences. This segmentation can help hotels tailor their marketing campaigns, services, and amenities to specific groups of guests for better customer satisfaction.  

***Cancellation Analysis:*** With information about whether a booking was canceled or not and factors that could influence cancellations (such as lead time, deposit type), hotels can analyze patterns of cancellations to identify common reasons why guests cancel their reservations. This analysis can help hotels implement strategies to reduce cancellations such as offering flexible cancellation policies or providing personalized offers to incentivize guests to keep their bookings.
These are just a few examples of how this dataset can be used creatively beyond simple descriptive analysis. Depending on the context and objectives of the analysis, there might be other interesting insights or applications that could arise from exploring this data further


***Acknowledgements***

**Original author:** Mesum Raza Hemani  
Data Source Kaggle.com
  
       

## Columns ##  
File: hotel_bookings.csv

| Column name | Description |  
|:--------------------- |:--------------------|
| hotel	| Indicates the type of hotel (resort or city). (Categorical)|  
is_canceled	| Specifies whether the booking was canceled or not (0=not canceled, 1=canceled). (Binary)  
|booking_date (*new*)| indicate de date of the reservation|
|lead_time	|Represents the number of days between the booking date and the arrival date. (Numerical)
|arrival_date_year|	Denotes the year of the |arrival date. (Categorical)
|arrival_date_month	|Indicates the month of the arrival date. (Categorical)
|arrival_date_week_number|	Specifies the week number in which guests arrived at the hotel. (Numerical)
|arrival_date_day_of_month|	Represents a specific day of arrival within a month. (Numerical)
|full_arrival_date (*new*)| indicates the full date|
|stays_in_weekend_nights|	Indicates how many nights (Saturday or Sunday) guests stayed or booked to stay at a hotel during weekends. (Numerical)|
|stays_in_week_nights|	Represents how many weeknights (Monday to Friday) guests stayed or booked to stay at a hotel during weekdays. (Numerical)|
|total_stays_in_nights (*new*)|	Represents how many nights in total guests stayed or booked to stay at a hotel . (Numerical)
|adults|	Indicates the number of adults included in each booking. (Numerical)
|children|	Indicates the number of children included in each booking. (Numerical)
|babies|	Indicates the number of babies included in each booking. (Numerical)
|meal|	Describes what type of meal was booked (Breakfast only, Half board, Full board, or Undefined/SC – no meal package). (Categorical)
|country|	Denotes the country-of-origin for each guest who made a reservation. (Categorical)
|market_segment|	Shows various market segments that individuals belong to when making reservations (e.g., Online Travel Agents, Offline Travel Agents, Corporate clients). (Categorical)
|distribution_channel|	Specifies different channels through which bookings were made (e.g., online travel agencies, direct bookings with hotels/tour operators, corporate arrangements). (Categorical)
|is_repeated_guest|	Indicates whether the guest is a repeated visitor (0=not repeated guest, 1=repeated guest). (Binary)
|previous_cancellations|	Represents the number of times guests previously canceled their bookings. (Numerical)
|previous_bookings_not_canceled|	Denotes the count of previous bookings made by guests that were not canceled. (Numerical)
|reserved_room_type|	Identifies the type of room initially reserved. (Categorical)
|assigned_room_type|	Identifies the type of room that was assigned to guests. (Categorical)
|booking_changes|	Represents the number of changes made to the booking. (Numerical)
|deposit_type|	Indicates the type of deposit made for the booking. (Categorical)
|agent|	Represents the ID of the travel agency that made the booking. (Categorical)
company|	Represents the ID of the company that made the booking. (Categorical)
|days_in_waiting_list|	Represents the number of days the booking was on the waiting list before being confirmed. (Numerical)
|customer_type|	Indicates the type of customer (e.g., transient, contract, group, or other). (Categorical)
|adr|	Represents the average daily rate (price per room) for the booking. (Numerical)
|required_car_parking_spaces|	Indicates the number of car parking spaces required by the guest. (Numerical)
|total_of_special_requests|	Represents the total number of special requests made by the guest (e.g., extra bed, room amenities). (Numerical)
|reservation_status|	Indicates the status of the reservation (e.g., canceled, checked-in, no-show). (Categorical)
|reservation_status_date|	Represents the date on which the reservation status was last updated. (Date)  



## Data Cleaning

**Modifications:**

* arrival_date_month changed from text to numerical value  
* addition column full_arrival_date  
* addition column booking_date
* addition column total_stays_in_nights
* removal of decimal in values for the columns agent and company  
* format change to ##,#0 for the values in column adr
* removal of all entries (716) with 0 nights stay and 0 adr  
* removal of all entries (111) with 0 adults and 0 child
* removal of outlayers from adr column
* add value 0 in column children where the value was left blank

creation of new CSV hotel_bookings_processed_data
creation of file Hotel_bookings_analysis


## Analysis

* creation of tab for numerical attributes analysis
