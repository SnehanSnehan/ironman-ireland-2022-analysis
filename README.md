🏊🚴🏃 Ironman Ireland 2022 – Performance Analysis

This project analyzes athlete performance data from the Ironman Ireland 2022 triathlon event. A total of 1,045 athletes who completed the race are included. The goal of this analysis is to understand how factors such as age, gender, and individual race segments (swim, bike, run) influence overall finishing time.

📌 Research Question

What factors affect race performance in Ironman Ireland 2022?

The analysis examines:

Influence of age

Differences across gender

Contribution of race segments to total finish time

📊 Dataset Description

The dataset contains information such as:

Athlete demographics → Age group, gender, country

Times for each event → Swim, bike, run

Overall completion time (HH:MM:SS)

Pre-processing steps included:

Converting time strings to numeric (hours)

Extracting numeric age values

Creating gender variable from age group codes

🔎 Analysis Summary
✅ 1. Distribution of Finish Times

Most athletes finish between 13–15 hours, with an average time of 13.5 hours.
The distribution is slightly right-skewed due to slower finishers (>17 hours).

✅ 2. Performance by Age Group

Professional athletes (MPRO, FPRO) are the fastest (≈ 9–10 hours).

Younger age groups (25–39) perform better than older categories.

F50–54 finishes slowest on average.

Largest participation: M40–44

✅ 3. Comparison of Race Segments

Bike takes the longest (median ≈ 5 hours)

Swim is shortest (≈ 1 hour)

Run takes 3–4 hours
Bike time shows the biggest performance variation among athletes.

✅ 4. Age & Performance Relationship

Positive relationship → older athletes finish slower

Trend holds for both genders

High variation → strong individual fitness differences

Males dominate participation (≈ 88%)

🏁 Key Findings
Factor	Observation
Age	Older athletes = longer finish times
Gender	Males slightly faster; participation heavily male
Segment difficulty	Bike is most time-consuming; largest performance spread
Experience	Professionals finish 3–4 hours faster
Average finisher	~13.5 hours; most finish 13–15 hours

Conclusion:
Age, experience level, and particularly bike performance are key drivers of overall Ironman results. Although age trends are clear, standout performances occur at all ages—showing that dedication and training strongly influence outcomes.

📁 Image Files

Plots are located under /images/:

plot1_finish_time_distribution.png

plot2_age_group_performance.png

plot3_segment_comparison.png

plot4_age_vs_performance.png

These visuals support the interpretation of finish distributions, age effect, segment contributions, and gender–age interactions.

🛠️ Technology Used

R

Tidyverse

ggplot2

dplyr

lubridate

🚀 How to Run

Clone repository

Install required R packages

Run the .Rmd / .R script

View generated plots in images/

📌 Author

Snehan
