🏊🚴🏃 Ironman Ireland 2022 — Performance Analysis (R)

This project analyzes Ironman Ireland 2022 race data to understand how
age, gender, and race segments (swim, bike, run) influence overall finishing times.
The analysis was carried out in R using tidyverse packages and visualized through multiple plots.

✅ Research Question

Which factors influence overall race performance in Ironman Ireland 2022?

✅ Dataset Overview

The dataset includes performance details for 1,045 athletes.

Each record contains:

Swim time (3.8 km)

Bike time (180 km)

Run time (42.2 km)

Overall completion time

Age group (AG)

Gender

Country

Times originally in HH:MM:SS were converted into numeric hours.

Data source: ironman (1).Rdata included in this repository

✅ Project Structure
/
├── README.md
├── ironman (1).Rdata
├── ironman_project.Rmd
├── ironman_report.html
└── plots/
      ├── age_group_performance.png
      ├── age_group_plot.png
      ├── age_vs_performance.png
      └── race_segments_comparison.png

✅ Tools & Packages Used
Category	Tools
Language	R
Libraries	dplyr, ggplot2, tidyr, lubridate
Output	HTML report, Plots
✅ Data Preparation

✔ Converted race times → numeric hours
✔ Extracted numerical ages from age groups
✔ Derived gender from age group codes
✔ Organized data for segment-wise analysis

✅ Key Plots & Insights
1️⃣ Distribution of Overall Finish Times

Most athletes finish between 13–15 hours, averaging ~13.5 hours.

📁 plots/age_group_plot.png

2️⃣ Average Finish Time by Age Group

Professional groups (MPRO, FPRO) are fastest (~9–10 hrs)

Age-group athletes slow progressively with age

📁 plots/age_group_performance.png

3️⃣ Race Segment Comparison

Bike is longest (~5 hours)

Run: ~3–4 hours

Swim: ~1 hour

📁 plots/race_segments_comparison.png

4️⃣ Age vs. Performance

Older athletes tend to finish slower.
Trend consistent in men and women.

📁 plots/age_vs_performance.png

✅ Key Findings
Factor	Observation
Age	Performance declines with age
Segment	Bike consumes the most time with highest variance
Experience	PRO athletes finish 3–4 hours faster
Gender	88% male participants; slightly faster

✅ Average finishing time ≈ 13.5 hours
✅ Most athletes finish within 13–15 hours

✅ How to Run

1️⃣ Clone this repo:

git clone https://github.com/SnehanSnehan/ironman-ireland-2022-analysis.git


2️⃣ Open ironman_project.Rmd in RStudio
3️⃣ Install required libraries
4️⃣ Knit to HTML

✅ Author

Snehan
2025-11-05
