 #🏊🚴🏃 Ironman Ireland 2022 — Performance Analysis (R)

This project explores the **Ironman Ireland 2022** race data and analyzes how
age, gender, and individual race segments (swim, bike, run) affect overall
finishing performance.  
The analysis is carried out in **R** using tidyverse libraries, and results are
presented with summary statistics and visualizations.

---

## ✅ Research Question
> **Which factors influence the overall race performance in Ironman Ireland 2022?**

---

## ✅ Dataset Overview

The dataset contains results from **1,045 athletes** who completed the event.

Each row represents an athlete with:
- Swim time (3.8 km)
- Bike time (180 km)
- Run time (42.2 km)
- Overall completion time
- Age group (AG)
- Gender
- Country

Times were originally stored in `HH:MM:SS` format and converted to numeric hours for analysis.

> Data source: Provided as `ironman.Rdata` within this repository.
---

## ✅ Tools & Packages Used

| Category | Tools |
|----------|-------|
| Language | R |
| Libraries | `dplyr`, `ggplot2`, `tidyr`, `lubridate` |
| Output | HTML report, Plots |

---

## ✅ Data Preparation

Steps performed:
- Converted all race times to **numeric hours**
- Extracted **numeric age** from age group identifier
- Generated **binary gender** variable from age group fields
- Reshaped data for segment-level comparison

---

## ✅ Key Plots & Insights

### 1️⃣ **Distribution of Overall Finish Times**
Most athletes finish between **13–15 hours**, with an average of **~13.5 hours**.

📁 `plots/dist_finish_times.png`

---

### 2️⃣ **Average Finish Time by Age Group**
Professional athletes (MPRO, FPRO) finish the fastest (~9–10 hrs).  
Among amateurs, performance decreases with age.

📁 `plots/age_group_times.png`

---

### 3️⃣ **Segment Time Comparison**
Bike segment takes the longest (~5 hours)  
Run ≈ 3–4 hours  
Swim ≈ 1 hour  

📁 `plots/segment_boxplot.png`

---

### 4️⃣ **Relationship Between Age & Performance**
Older athletes tend to take longer to finish.  
This upward trend is consistent for both men and women.

📁 `plots/age_vs_perf.png`

---

## ✅ Key Findings

| Factor | Observation |
|--------|-------------|
| Age | Performance declines with age |
| Segment | Bike consumes most time & has largest variation |
| Experience | PRO athletes finish 3–4 hours faster |
| Gender | Males = 88% of participants; slightly faster average time |

✅ **Average finishing time ≈ 13.5 hours**  
✅ Performance clusters around 13–15 hours  

---

## ✅ How to Run

1. Clone repo:
```bash
git clone https://github.com/SnehanSnehan/ironman-ireland-2022-analysis.git
Open R or RStudio

Install required libraries (if needed):

install.packages(c("ggplot2", "dplyr", "tidyr", "lubridate"))


Run:

source("code/analysis.R")


Check generated plots in the plots/ folder
