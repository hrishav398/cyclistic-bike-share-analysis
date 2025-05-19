

# Cyclistic Bike-Share Analysis: How Does a Bike-Share Navigate Speedy Success?

This is my capstone project for the **Google Data Analytics Professional Certificate**, where I analyzed Cyclistic’s 2019 bike-share trip data to uncover behavioral trends and help guide the company’s marketing strategy. The goal: understand how **casual riders** differ from **annual members**, and identify ways to convert more casual users into paying members.

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
![Riders by User Type](visuals/Riders per user type.png)

### 2. Average Ride Duration by User Type
![Average Ride Duration](visuals/avg ride length per user type.png)

### 3. Ride Duration by Day and User Type
![Ride by Day](visuals/avg ride length by day and user type.png)

###4. 
![Ride by Day](visuals/riders per week day trend.png)

### 5. Rides by Hour of Day
![Hourly Rides](visuals/Ride Count by hour of the day and user type.png)

### 6. Top 10 Starting Stations
![Top Stations](visuals/station ride counts.png)

### 7. Ride Duration by Birth Year (data not cleaned)
![Ride by Birth Year](visuals/avg duration per birth year_mistake.png)

### 8. Ride Duration by Birth Year (Cleaned)
![Ride by Birth Year](visuals/avg duration per birth year corrected.png)

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


