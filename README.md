# ✈️ Airline Operations Analysis using Python


## 📌 Project Overview
This project performs an end-to-end exploratory and analytical study **(5.82M)** rows of airline operations, focusing on flight delays, cancellations, airline performance, airport congestion, and traffic patterns. 

Using Python and data analysis libraries, the project extracts actionable insights that help understand:

- Which airlines are most reliable
- Which airports experience the highest delays
- How delays vary by time, route, and season
- Major reasons behind flight cancellations

The insights generated in Python can be exported and visualized interactively in Power BI.

## ❓ The Questions

Below are the questions I want to answer in my Project -

1. Which Airlines are Cancelled mostly and what are the Cancellation reasons?
2. Which routes are most busy?
3. What are the Arrival & Departure Delays by Airlines & Airports?
4. What are the Arrival & Departure Delays by hour of the day?


## 🎯 Objectives
- Analyze arrival and departure delays
- Identify on-time vs delayed airline performance
- Study flight cancellations and their reasons
- Understand hourly, daily, and monthly traffic trends
- Identify high-traffic and high-delay routes
- Prepare aggregated datasets for dashboarding

## 📊 Dataset Description
The dataset contains commercial flight records with the following key attributes:

| Attribute | Description |
|-----------|-------------|
| Flight Date | Year, Month, Day, Hour |
| Airline Codes | IATA, Airline |
| Origin & Destination Airports | Origin Airport, Destination Airport |
| Scheduled and Actual Times | Scheduled Time, Departure Delay, Departure Time, Taxi Out, Wheels Off etc|
| Arrival & Departure Delays | Scheduled Arrival, Elapsed Time, Departure Time, Arrival Delay, Taxi In, Wheels In etc|
| Cancellation Status and Reasons | Cancelled, Cancelled Reason |
| Distance Travelled | Distance, Airtime |

The dataset is pre-cleaned for analysis by handling missing values, invalid time formats, and inconsistent categorical data. 

## 🛠️ Tools & Technologies Used

### Programming & Libraries
- **Python**
- **pandas** – data manipulation
- **numpy** – numerical operations
- **matplotlib** – static visualizations

# Dataset File 
- **Source:** https://mavenanalytics.io/data-playground/airline-flight-delays
- **Size:** 5.82M rows
- **File Size:** ~500MB


## 🔄 Data Cleaning & Preparation
Key preprocessing steps include:

- Data Preparation


- Extracting Month Names from Month Number Data

<img width="910" height="102" alt="Extracting Month" src="https://github.com/user-attachments/assets/83ffa9d7-e8a0-4f04-813c-d83b20e13561" />

- Extracting hour of day from scheduled times

<img width="837" height="207" alt="Extracting Hour" src="https://github.com/user-attachments/assets/50564c38-52cf-4205-9ded-cb291b3ce7ab" />

- Handling: NaN / None / NaT values / Empty / whitespace strings
- Tthe NULL/None values in some columns were related to Cancelled Flights. Overall these values were less than 2% of all the rows. So, I didn't remove them as these were not changing the key metrics by bigger margins


- Standardizing month order using categorical data
- Creating derived metrics (on-time %, cancellation rate)


### You can find the complete [Data Cleaning & Preparation](https://github.com/chennakesava2183/Airline-Operations-Analysis-using-Python/blob/a96951cfa505f9834a8c8d15a8348ec5561e4bb1/Data%20Loading%20%26%20Cleaning.ipynb "Data Cleaning & Preparation") in this path.

## 📈 Key Analyses Performed

### 1️⃣ Delay Analysis
### Median Arrival Delay by Airline

Visualize Data -
 <img width="961" height="144" alt="Delay by Airlines" src="https://github.com/user-attachments/assets/5c457a43-c1a7-437e-9f44-3ae063887a21" />


Results -

<img width="1463" height="910" alt="Delay by Airlines Chart" src="https://github.com/user-attachments/assets/5d69c48c-031b-405b-8d6c-96a732f175ab" />



### Median Departure Delay by Hour of Day 




### Distance vs Scheduled Time Scatter Analysis



### 2️⃣ Cancellation Analysis
 ### Cancellation Rate by Airline 
 
 Visualize Data -
 <img width="1345" height="43" alt="Airlines Cancellation" src="https://github.com/user-attachments/assets/2bf6466f-932a-41cc-ab1c-e3ccf195483d" />


 Results -
 
<img width="1464" height="583" alt="Airlines Cancellation Chart" src="https://github.com/user-attachments/assets/b6c5f506-a4ad-4ff2-bf40-e6051fbce71e" />

### Cancellation Reasons Distribution



### Cancellations by Month



### Cancellations by Hour of Day


### Cancellations by Route



### 3️⃣ Airline Performance


### On-time performance percentage




### 4️⃣ Airport & Route Insights

### Busiest airports by flight volume

<img width="1490" height="590" alt="Busiest Air Routes" src="https://github.com/user-attachments/assets/199ed0f3-cf3b-4fdf-9f51-d4b2066dd2fe" />


### Most congested destination airports



### You can find the [Metrics & Calculations](https://github.com/chennakesava2183/Airline-Operations-Analysis-using-Python/blob/a96951cfa505f9834a8c8d15a8348ec5561e4bb1/Metric%20Calculations.ipynb "Metrics & Calculations") & [Visualizations](https://github.com/chennakesava2183/Airline-Operations-Analysis-using-Python/blob/7a7a78edd828aacc4f640a20ae77424fd57f98ac/Visualizations.ipynb " Visualizations") & [Complete Scripts](https://github.com/chennakesava2183/Airline-Operations-Analysis-using-Python/blob/8472b0e3b9bf1203c6427d3d905abf44bab7090c/Airlines_Analysis.ipynb " Full Python Script") here


## 📊 Visualizations Created
- Line charts (hourly and monthly trends)
- Bar and horizontal bar charts
- Scatter plots (distance vs delay)
- Pie charts (cancellation reasons)

**All charts are:**
- Properly labeled
- Scaled for readability


## ✅ Key Business Insights
- Delta Airlines & Alaska Airlines consistently maintain lower median delays
- Best On-Time Performance: Delta Airlines with 70% on-time rate
- Peak delays occur during evening to late evening hours
- Less flights are Cancelled from Midninght to early Morning hours
- Most Flights are Cancelled in February and in September very less flights are Cancelled.
- Weather-related cancellations(54%) dominate over Technical issues
- Busiest Route: San Francisco - Los Angeles with nearly 14k Flights
- High-traffic routes often have the highest cancellations
- Southwest Airlines has 16k Cancellations

 ## 💡 Business Recommendations
**For Airlines:**
- Enquire why most Cancellations are happening for the Boston - New York Route
- Increase buffer time for February operations

**For Passengers:**
- Book morning flights to minimize delay risk
- Avoid Spirit Airlines if on-time arrival is critical
- Purchase travel insurance for winter months

## ❓ Challenges I Faced

This project was not without its challenges, but it provided good learning opportunities:

   - Data Inconsistencies: Handling missing or inconsistent data entries requires careful consideration and thorough data-cleaning techniques to ensure the integrity of the analysis.
   - Complex Data Visualization: Designing effective visual representations of complex datasets was challenging but critical for conveying insights clearly and compellingly.
   - Balancing Breadth and Depth: Deciding how deeply to dive into each analysis while maintaining a broad overview of the data landscape required constant balancing to ensure comprehensive coverage without getting lost in details.

## 👤 Author
**Chenna Kesava Kumar Bonu**  
*Data Analyst | Python | Power BI | SQL | Excel*

## 📜 License
This project is for educational and portfolio purposes.

