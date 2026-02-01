# ✈️ Airline Operations Analysis using Python

## 📌 Project Overview
This project performs an end-to-end exploratory and analytical study of airline operations, focusing on flight delays, cancellations, airline performance, airport congestion, and traffic patterns. 

Using Python and data analysis libraries, the project extracts actionable insights that help understand:

- Which airlines are most reliable
- Which airports experience the highest delays
- How delays vary by time, route, and season
- Major reasons behind flight cancellations

The insights generated in Python can be exported and visualized interactively in Power BI.

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
https://mavenanalytics.io/data-playground/airline-flight-delays

## 🔄 Data Cleaning & Preparation
Key preprocessing steps include:

- Data Preparation

<img width="1389" height="405" alt="Data Preparation" src="https://github.com/user-attachments/assets/5151c3d8-8ca8-453e-bd5d-4cdca3ab09bf" />

- Extracting Month Names from Month Number Data

<img width="910" height="102" alt="Extracting Month" src="https://github.com/user-attachments/assets/83ffa9d7-e8a0-4f04-813c-d83b20e13561" />

- Extracting hour of day from scheduled times

<img width="837" height="207" alt="Extracting Hour" src="https://github.com/user-attachments/assets/50564c38-52cf-4205-9ded-cb291b3ce7ab" />

- Handling: NaN / None / NaT values / Empty / whitespace strings

<img width="594" height="825" alt="Data Cleaning" src="https://github.com/user-attachments/assets/7b608800-c74c-42bb-8e92-3d7eea953468" />

- Selective row removal (`dropna(subset=...)`)

<img width="817" height="170" alt="Data Cleaning 2" src="https://github.com/user-attachments/assets/7adcc0ae-cd10-4ab6-9252-1666407c519b" />

<img width="925" height="153" alt="Data Combined" src="https://github.com/user-attachments/assets/9ea9d4d3-bda7-4aa9-adb7-ae33ee3a9448" />

- Standardizing month order using categorical data
- Creating derived metrics (on-time %, cancellation rate)

## 📈 Key Analyses Performed

### 1️⃣ Delay Analysis
### Median Arrival Delay by Airline

Visualize Data -
 <img width="961" height="144" alt="Delay by Airlines" src="https://github.com/user-attachments/assets/5c457a43-c1a7-437e-9f44-3ae063887a21" />


Results -

<img width="1463" height="910" alt="Delay by Airlines Chart" src="https://github.com/user-attachments/assets/5d69c48c-031b-405b-8d6c-96a732f175ab" />



### Median Departure Delay by Hour of Day 

Visualize Data -
<img width="975" height="609" alt="Delay by Hour" src="https://github.com/user-attachments/assets/38804db5-2faf-4dd6-93d6-0905c3b80ecb" />


Results -

<img width="1466" height="545" alt="Delay by Hour Chart" src="https://github.com/user-attachments/assets/15e845a7-4afb-44cb-ba64-995ccf24e0e1" />



### Distance vs Scheduled Time Scatter Analysis

 <img width="1291" height="758" alt="Distance and Schedule Time Scatter" src="https://github.com/user-attachments/assets/4b88eae2-58c2-46df-b0eb-d94e9db6f6e4" />



### 2️⃣ Cancellation Analysis
 ### Cancellation Rate by Airline 
 
 Visualize Data -
 <img width="1345" height="43" alt="Airlines Cancellation" src="https://github.com/user-attachments/assets/2bf6466f-932a-41cc-ab1c-e3ccf195483d" />


 Results -
 
<img width="1464" height="583" alt="Airlines Cancellation Chart" src="https://github.com/user-attachments/assets/b6c5f506-a4ad-4ff2-bf40-e6051fbce71e" />

### Cancellation Reasons Distribution

<img width="668" height="690" alt="Cancellation Reasons" src="https://github.com/user-attachments/assets/9ac74535-e8ba-49f2-ad91-7f6a8ce88427" />


### Cancellations by Month

Visualize -

<img width="1133" height="583" alt="Cancelled Flights per Month" src="https://github.com/user-attachments/assets/3ac4072a-ec96-4ee9-aae2-88be4e69722a" />

Results -

<img width="1389" height="590" alt="Cancelled Flights per Month Chart" src="https://github.com/user-attachments/assets/7891af0d-b379-4daa-8b4c-21309d42ae82" />


### Cancellations by Hour of Day

<img width="1489" height="590" alt="Cancelled by Hour" src="https://github.com/user-attachments/assets/868feb9c-94a4-4929-9de8-229edfe69499" />

### Cancellations by Route

Visualize Data - 

<img width="1458" height="114" alt="Cancelled Route 1" src="https://github.com/user-attachments/assets/fa670924-d02d-4238-b21c-d9af2fdbcbbf" />

Results - 

<img width="1489" height="590" alt="Cancelled Routes" src="https://github.com/user-attachments/assets/18a1fa66-80da-441b-90e9-177fca30e8f3" />



### 3️⃣ Airline Performance


### On-time performance percentage

Visualize Data -

<img width="649" height="667" alt="On Time Airline" src="https://github.com/user-attachments/assets/caed7afb-beba-4ce5-ad11-22ce1c3fc697" />

Results -

<img width="1386" height="547" alt="On Time Airline Chart" src="https://github.com/user-attachments/assets/701002d3-eb6a-44b3-9a0f-8917d3a13f0a" />



### 4️⃣ Airport & Route Insights

### Busiest airports by flight volume

<img width="1490" height="590" alt="Busiest Air Routes" src="https://github.com/user-attachments/assets/199ed0f3-cf3b-4fdf-9f51-d4b2066dd2fe" />


### Most congested destination airports

<img width="1650" height="590" alt="Median Taxi In by Airports" src="https://github.com/user-attachments/assets/59a5f192-deaa-4957-8685-caf7a92f3ad4" />



## 📊 Visualizations Created
- Line charts (hourly and monthly trends)
- Bar and horizontal bar charts
- Scatter plots (distance vs delay)
- Pie charts (cancellation reasons)

**All charts are:**
- Properly labeled
- Scaled for readability


## ✅ Key Business Insights
- Certain airlines consistently maintain lower median delays
- Peak delays occur during evening to late evening hours
- Less flights are Cancelled from Midninght to early Morning hours
- Most Flights are Cancelled in February and in September very less flights are Cancelled.
- Weather-related cancellations dominate over technical issues
- High-traffic routes do not always have the highest delays
- High-traffic routes often have the highest cancellations

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

