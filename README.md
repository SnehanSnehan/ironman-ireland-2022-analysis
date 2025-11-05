# 🏊‍♂️🚴‍♂️🏃‍♂️ Ironman Ireland 2022: Performance Analysis

A data-driven exploration of performance factors in the Ironman Ireland 2022 triathlon competition.

---

## 📋 Overview

This project analyzes race data from **1,045 athletes** who completed Ironman Ireland 2022. The analysis explores how age, gender, and race segments influence overall performance in this challenging endurance event.

**Ironman Distance:**
- 🏊‍♂️ Swim: 3.8 km
- 🚴‍♂️ Bike: 180 km  
- 🏃‍♂️ Run: 42.2 km (marathon)

---

## 🔍 Research Question

**What factors affect race performance in Ironman Ireland 2022?**

---

## 📊 Key Findings

| Metric | Finding |
|--------|---------|
| **Average Finish Time** | 13.5 hours (most athletes: 13-15 hours) |
| **Age Impact** | Performance declines with age, though variation is substantial |
| **Critical Segment** | Bike portion takes longest (~5 hours avg) with highest variation |
| **Professional Advantage** | Pro athletes finish 3-4 hours faster than age-groupers |
| **Gender Split** | 88% male, 12% female; males slightly faster on average |

---

## 📁 Repository Structure
```
ironman-ireland-2022-analysis/
├── README.md                           # Project documentation
├── ironman (1).Rdata                  # Raw race data
├── ironman_project.Rmd                # R Markdown analysis script
├── ironman_report.html                # Generated HTML report
└── plots/
    ├── age_group_performance.png      # Age group comparison
    ├── age_group_plot.png             # Age group distribution
    ├── age_vs_performance.png         # Age-performance relationship
    └── race_segments_comparison.png   # Segment breakdown
```

---

## 🛠️ Tools & Packages Used

| Category | Tools |
|----------|-------|
| **Language** | R |
| **Libraries** | `dplyr`, `ggplot2`, `tidyr`, `knitr` |
| **Output** | HTML report, PNG plots |

---

## 🔧 Data Preparation

Steps performed:
- ✅ Converted all race times from **HH:MM:SS** to **numeric hours**
- ✅ Extracted **numeric age** from age group categories
- ✅ Generated **binary gender** variable from age group codes
- ✅ Reshaped data for segment-level comparison

---

## 📈 Key Plots & Insights

### 1️⃣ **Distribution of Overall Finish Times**
Most athletes finish between **13–15 hours**, with an average of **~13.5 hours**.  
📁 `plots/age_group_performance.png`

---

### 2️⃣ **Average Finish Time by Age Group**
- Professional athletes (MPRO, FPRO) finish fastest (~9–10 hrs)
- Among age-groupers, performance decreases with age
- F50-54 shows longest average time

📁 `plots/age_group_plot.png`

---

### 3️⃣ **Segment Time Comparison**
- **Bike** segment takes the longest (~5 hours)
- **Run** takes ~3–4 hours  
- **Swim** is shortest (~1 hour)
- Bike shows highest performance variation

📁 `plots/race_segments_comparison.png`

---

### 4️⃣ **Age vs Performance Relationship**
- Clear positive correlation: older athletes take longer
- Pattern consistent across both genders
- Individual variation remains substantial
- Some 50+ and 60+ athletes still achieve competitive times

📁 `plots/age_vs_performance.png`

---

## 🚀 Usage

### Prerequisites
- R (version 3.6 or higher)
- Required packages: `ggplot2`, `dplyr`, `tidyr`, `knitr`

### Running the Analysis
1. Clone this repository
2. Open `ironman_project.Rmd` in RStudio
3. Knit the document to reproduce the analysis
4. View the generated `ironman_report.html`
```r
# Install required packages if needed
install.packages(c("ggplot2", "dplyr", "tidyr", "knitr"))

# Load the data
load("ironman (1).Rdata")
```

---

## 💡 Conclusions

This analysis reveals several factors affecting Ironman performance:

- **Age matters**, but isn't deterministic — training and individual fitness vary widely
- **Bike segment** is the most time-consuming and variable, suggesting it's key for overall performance
- **Professional athletes** demonstrate significantly superior performance across all segments
- **Gender representation** is uneven, with males comprising the vast majority of participants

The average finisher completes the race in **13.5 hours**, providing a useful benchmark for athletes planning their race strategy.

---

## 👤 Author

**Snehan**  
📅 November 5, 2025

---

## 📄 License

This project is for educational and analytical purposes.

---

## 🤝 Contributing

Feel free to open issues or submit pull requests if you have suggestions for improving the analysis.

---

**⭐ If you find this analysis useful, consider starring the repository!**
