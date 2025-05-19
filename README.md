

# Cyclistic Bike-Share Analysis: How Does a Bike-Share Navigate Speedy Success?

This is my capstone project for the **Google Data Analytics Professional Certificate**, where I analyzed Cyclistic’s 2019 bike-share trip data to uncover behavioral trends and help guide the company’s marketing strategy. The goal: understand how **casual riders** differ from **annual members**, and identify ways to convert more casual users into paying members.
This project was built using Q1, Q2, Q3, and Q4 of 2019 data from Cyclistic (Divvy) — a full year of ride logs covering millions of bike-share trips across Chicago. I chose to work with the complete 2019 dataset because it provided a rich, seasonal view of rider behavior, which I believed was essential for uncovering trends beyond surface-level summaries.
During the analysis, I encountered a few surprises that weren’t obvious until I visualized the data:
I discovered that some trips had negative durations, and others lasted more than 24 hours, a data quality issue. I filtered these out to ensure the average duration metrics were meaningful.
The line plot of average ride duration by birth year unexpectedly revealed riders born as early as 1760. These were system errors or placeholders for missing data. Initially, I thought the data was fine, but that plot helped uncover how unrealistic some entries were. I filtered these out by retaining only birth years from 1919 to 2004, representing riders roughly aged 15 to 100, which is a more plausible range for bike users.
This capstone project helped me strengthen my Python and data visualization skills, but more importantly, it helped me:

- Think critically about data integrity

- Connect metrics to real-world decisions

- Communicate insights in a way that non-technical stakeholders could understand and act on

- Every chart I included wasn’t just about making something look good — it was about answering a specific business question with evidence-backed storytelling.


---

##  Business Objective

Cyclistic’s marketing team wants to increase the number of annual memberships. To support this effort, I conducted a detailed analysis to answer:

> "How do annual members and casual riders use Cyclistic bikes differently?"

---

##  Key Insights

| Insight | Explanation |
|--------|-------------|
| **Ride Length** | Casual riders take significantly longer trips than members |
| **Day of Week** | Casual rides peak on weekends; members ride steadily throughout the week |
| **Time of Day** | Casual users ride more in the afternoon and evening; members peak around morning/evening commutes |
| **Stations** | Casual riders start trips most often at tourist-heavy downtown locations |
| **Age Patterns** | Most riders were born between 1980 and 2000; older outliers were removed for accuracy |

---

## Visualizations

Charts created using Python (Seaborn + Matplotlib) and available in the `/visuals/` folder.

### 1. Riders by User Type
![Riders by User Type](Visuals/Riders%20per%20user%20type.png)

### 2. Average Ride Duration by User Type
![Average Ride Duration](Visuals/avg%20ride%20length%20per%20user%20type.png)

### 3. Ride Duration by Day and User Type
![Ride by Day](Visuals/avg%20ride%20length%20by%20day%20and%20user%20type.png)

### 4. Riders per day of the week 
![Ride by Day](Visuals/riders%20per%20week%20day%20trend.png)

### 5. Rides by Hour of Day
![Hourly Rides](Visuals/Ride%20Count%20by%20hour%20of%20the%20day%20and%20user%20type.png)

### 6. Top 10 Starting Stations
![Top Stations](Visuals/station%20ride%20counts.png)

### 7. Ride Duration by Birth Year (data not cleaned)
![Ride by Birth Year](Visuals/avg%20duration%20per%20birth%20year_mistake.png)

### 8. Ride Duration by Birth Year (Cleaned)
![Ride by Birth Year](Visuals/avg%20duration%20per%20birth%20year%20corrected.png)

- 

---

##  Process Followed

### ASK
- What business problem am I trying to solve?
- What do stakeholders need to know to support a marketing campaign?

### PREPARE
- Downloaded and merged all 4 quarters of 2019 Cyclistic trip data
- Cleaned and formatted columns for consistency

### PROCESS
- Removed invalid entries (negative durations, unrealistic birth years)
- Created new features like `ride_length`, `hour`, and `day_of_week`

### ANALYZE
- Compared usage patterns between user types across time, age, and location

### SHARE
- Built a clean, modular Python notebook with commentary and visualizations
- Published findings and charts to GitHub

### ACT
- Recommend targeting casual riders with:
  - Weekend promotions
  - QR code sign-ups at high-traffic stations
  - Free trial or discount offers during peak hours

---

## Tools Used

- Python (pandas, matplotlib, seaborn)
- Google Colab
- GitHub

---

## Dataset

- Source: Motivate International Inc. / Divvy (via [Divvy Open Data Portal](https://divvybikes.com/system-data))
- Data license: [Link](https://www.divvybikes.com/data-license-agreement)

---


