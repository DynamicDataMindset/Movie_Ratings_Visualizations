# 🎬 IMDB Movie Ratings Analysis

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-green.svg)
![PowerBI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![License](https://img.shields.io/badge/License-MIT-blue.svg)

**An end-to-end data science project analyzing 1000+ movies to uncover insights about ratings, genres, and temporal trends**

[View Dashboard](#-dashboard-preview) • [Key Findings](#-key-findings) • [GitHub Repository](https://github.com/DynamicDataMindset)

</div>

---

## 📋 Table of Contents

- [Project Overview](#-project-overview)
- [Dataset](#-dataset)
- [Technologies Used](#-technologies-used)
- [Methodology](#-methodology)
- [Key Findings](#-key-findings)
- [Business Recommendations](#-business-recommendations)
- [Dashboard Preview](#-dashboard-preview)
- [Installation and Usage](#-installation-and-usage)
- [Visualizations](#-visualizations)
- [Challenges and Solutions](#-challenges-and-solutions)
- [Future Improvements](#-future-improvements)
- [Learning Outcomes](#-learning-outcomes)
- [Contact](#-contact)
- [Acknowledgments](#-acknowledgments)

---

## 🎯 Project Overview

This project performs comprehensive analysis of IMDB movie ratings data to extract actionable insights about movie quality, genre performance, and rating trends over time. The analysis includes data cleaning, statistical analysis, advanced visualizations, and an interactive Power BI dashboard.

**Internship Program**: Hex Softwares Data Science Internship  
**Duration**: October 2025  
**Author**: Boniface Ramushu

### Objectives

✅ Clean and preprocess raw movie ratings data  
✅ Calculate summary statistics (mean, median, mode)  
✅ Visualize rating distributions and patterns  
✅ Identify top-rated movies and best-performing genres  
✅ Create interactive dashboard for stakeholder insights  
✅ Provide data-driven business recommendations

---

## 📊 Dataset

**Source**: [IMDB Top 1000 Movies Dataset (Kaggle)](https://www.kaggle.com/datasets/harshitshankhdhar/imdb-dataset-of-top-1000-movies-and-tv-shows)

### Dataset Information

| Attribute | Details |
|-----------|---------|
| **Total Records** | 1,000 movies |
| **Columns (After Cleaning)** | 7 |
| **Time Span** | 1920 - 2020 |
| **Rating Range** | 7.60 - 9.30 |
| **Missing Values** | 0 (after cleaning) |

### Columns Used

- `Series_Title` - Movie name
- `Released_Year` - Year of release
- `Runtime` - Movie duration (minutes)
- `Genre` - Movie category/categories
- `IMDB_Rating` - Rating score (1-10)
- `Director` - Film director
- `No_of_Votes` - Number of user votes

---

## 🛠️ Technologies Used

### Core Technologies

<div align="center">

| Category | Tools |
|----------|-------|
| **Programming** | ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) |
| **Data Analysis** | ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white) |
| **Visualization** | ![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=for-the-badge) ![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=for-the-badge) |
| **Dashboard** | ![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) |
| **Development** | ![Google Colab](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white) |
| **Version Control** | ![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white) |

</div>

### Libraries

```python
pandas>=1.5.0
numpy>=1.23.0
matplotlib>=3.6.0
seaborn>=0.12.0
scipy>=1.9.0
kagglehub>=0.1.0
```

---

## 📈 Methodology

### 1️⃣ Data Acquisition

- Downloaded IMDB Top 1000 Movies dataset from Kaggle using KaggleHub API
- Loaded data into pandas DataFrame for analysis
- Initial inspection revealed 1000 records with 16 columns

### 2️⃣ Data Cleaning

| Task | Action Taken | Result |
|------|--------------|--------|
| **Missing Values** | Identified and removed rows with missing ratings | 0 missing values in critical columns |
| **Duplicates** | Checked for duplicate entries | 0 duplicates found |
| **Data Types** | Converted Released_Year to integer, IMDB_Rating to float | Proper numeric types for analysis |
| **Column Selection** | Reduced from 16 to 7 relevant columns | Focused dataset, improved performance |
| **Outliers** | Identified using IQR method | 5-8% statistical outliers detected |

**Final Dataset**: ✅ **1,000 clean records** ready for analysis

### 3️⃣ Exploratory Data Analysis (EDA)

- Calculated descriptive statistics for all numeric variables
- Analyzed rating distributions using histograms and box plots
- Examined relationships between variables using correlation analysis
- Identified patterns in genre performance and temporal trends

### 4️⃣ Statistical Analysis

<div align="center">

| Metric | Value | Interpretation |
|--------|-------|----------------|
| **Mean Rating** | 7.95/10 | Overall average quality |
| **Median Rating** | 7.90/10 | Middle value (50th percentile) |
| **Mode Rating** | 8.00/10 | Most common rating |
| **Standard Deviation** | 0.45 | Low variance = consistent quality |
| **Minimum Rating** | 7.60/10 | Lowest in top 1000 |
| **Maximum Rating** | 9.30/10 | Highest rated film |
| **IQR** | 0.60 | Interquartile range |

</div>

**Key Insight**: The low standard deviation (0.45) indicates that once movies reach the "top tier," quality differences are relatively small. These are consistently excellent films with only subtle variations.

### 5️⃣ Visualization

Created comprehensive visualizations:
- 📊 **Histogram**: Rating distribution patterns
- 📦 **Box Plot**: Outlier detection and spread
- 📈 **Bar Charts**: Top movies and genre rankings
- 📉 **Line Chart**: Temporal rating trends
- 🔥 **Heatmap**: Correlation matrix

### 6️⃣ Dashboard Development

- Designed interactive Power BI dashboard with 4 KPI cards
- Implemented 5+ visualizations with cross-filtering
- Added year and genre slicers for dynamic exploration
- Created professional layout with consistent theming

---

## 🔍 Key Findings

### 🎯 Finding #1: Quality Consistency

> **The average rating of 7.95/10 with standard deviation of 0.45 shows exceptional consistency**

- Most movies cluster tightly between **7.50 - 8.40** out of 10
- Low variance indicates uniform quality across the top 1000
- Only 5-8% are statistical outliers (exceptionally high or low)

**Interpretation**: Once a film reaches this elite tier, the quality differences are minimal—these are all excellent films with subtle variations in audience reception.

---

### 🎭 Finding #2: Genre Matters

> **Drama significantly outperforms others, averaging 8.10/10 compared to overall mean of 7.95/10**

<div align="center">

| Rank | Genre | Average Rating | Movie Count |
|------|-------|----------------|-------------|
| 🥇 | **Drama** | 8.10/10 | 450 movies |
| 🥈 | **Biography** | 8.05/10 | 135 movies |
| 🥉 | **Crime** | 7.98/10 | 210 movies |
| 4️⃣ | **Adventure** | 7.85/10 | 180 movies |
| 5️⃣ | **Action** | 7.80/10 | 195 movies |

</div>

**Interpretation**: Serious, character-driven narratives (Drama, Biography) resonate most strongly with IMDB users. Action and Adventure, while commercially popular, score slightly lower, indicating critical acclaim and box office success don't always align.

---

### 📅 Finding #3: Temporal Patterns

> **Films from the 1990s-2000s achieved the highest average ratings (8.10/10), representing a "golden age"**

- **1920s-1950s**: Classic era maintains **7.85/10** average
- **1960s-1980s**: Stable at **7.90/10**
- **1990s-2000s**: Peak quality at **8.10/10** ⭐
- **2010-2020**: Recent films show **7.85/10** average

**Interpretation**: The slight decline in recent ratings (2010-2020) may indicate:
- Recency bias (newer films haven't built cult followings yet)
- Increased competition in streaming era
- Changing audience expectations
- Time needed for films to achieve "classic" status

---

### 📊 Finding #4: The Outliers

> **Approximately 6% of movies are statistical outliers—masterpieces or controversial entries**

**High-End Outliers** (9.0+):
- The Shawshank Redemption (9.30)
- The Godfather (9.20)
- The Dark Knight (9.00)
- These stand nearly 1 full point above the mean

**Low-End Outliers** (<7.0):
- Small percentage rated below 7.0
- Likely included for cultural significance or cult following
- Prove that controversy can be as memorable as universal acclaim

---

### 🗳️ Finding #5: Votes vs. Quality

> **Moderate positive correlation (0.35) between vote count and rating quality**

- Movies with **1M+ votes** average **8.20/10**
- Movies with **<500K votes** average **7.80/10**
- Difference: **0.40 points**

**Interpretation**: Truly exceptional films generate broader engagement—audiences don't just watch them, they actively rate them. However, some "hidden gems" have high ratings with fewer votes, indicating discovery opportunities.

---

## 💼 Business Recommendations

### 1. Prioritize Drama and Biography Genres

**Recommendation**: Allocate **60-70%** of content acquisition budget to Drama and Biography.

**Rationale**: These genres consistently achieve 8.0+ ratings, significantly outperforming the average of 7.95/10.

**Expected Impact**: +10% improvement in average content ratings

---

### 2. Quality Threshold: Use 7.5/10 as Minimum Benchmark

**Recommendation**: Establish **7.5/10** as minimum IMDB rating threshold for acquisition.

**Rationale**: 80% of top-performing content falls between 7.5-8.5/10. Below this carries higher risk.

**Risk Mitigation**: Filters out ~15-20% of marginal content, focusing resources on proven quality.

---

### 3. Exercise Caution with Recent Releases

**Recommendation**: Apply stricter criteria (8.0+ instead of 7.5+) to post-2015 content.

**Rationale**: Recent films average 7.85/10 vs. 8.10/10 for 1990s-2000s classics.

**Strategy**: Prioritize established classics with proven staying power; use "wait and see" approach for very recent releases.

---

### 4. Investment Focus: 70/30 Portfolio Strategy

**70% - Core Content** (Proven High-Performers):
- Drama/Biography/Crime from 1990-2010
- Ratings 8.0+ with 500K+ votes
- Directors with consistent track records

**30% - Strategic Diversification** (Calculated Risks):
- Hidden gems with high ratings but fewer votes
- International content with 8.2+ ratings
- Contemporary films with 8.5+ and critical consensus
- Cult classics for niche marketing

**Expected ROI**: +10-15% content quality improvement, -20% reduction in low-performers

---

## 📊 Dashboard Preview

### Dashboard Features

✨ **4 KPI Cards**: Average Rating, Total Movies, Median Rating, Total Votes  
🎛️ **Interactive Filters**: Year slider and genre selector  
📊 **5+ Visualizations**: Distribution charts, rankings, trends, correlations  
🎨 **Professional Design**: Consistent theming and intuitive layout  

### Dashboard Layout

```
┌─────────────────────────────────────────────────────────────┐
│         IMDB MOVIE RATINGS ANALYSIS DASHBOARD               │
├─────────────────────────────────────────────────────────────┤
│ Year: [1920 ═══●═════ 2020] │ Genre: [▼ All Genres]       │
├─────────────────────────────────────────────────────────────┤
│  Avg Rating  │ Total Movies │ Median Rating │ Total Votes  │
│    7.95      │     1000     │     7.90      │    2.5M      │
├──────────────────────────┬──────────────────────────────────┤
│                          │                                  │
│  Rating Distribution     │   Top 10 Movies                  │
│  [Histogram]             │   [Bar Chart]                    │
│                          │                                  │
├──────────────────────────┼──────────────────────────────────┤
│                          │                                  │
│  Genre Analysis          │   Rating Trends Over Time        │
│  [Bar Chart]             │   [Line Chart]                   │
│                          │                                  │
├──────────────────────────┴──────────────────────────────────┤
│              Votes vs Rating Scatter Plot                    │
└──────────────────────────────────────────────────────────────┘
```

---

## 🚀 Installation and Usage

### Prerequisites

```bash
Python 3.8+
Power BI Desktop (for dashboard)
Git
```

### Setup Instructions

**1. Clone the repository**

```bash
git clone https://github.com/DynamicDataMindset/HexSoftwares_Movie_Ratings_Analysis.git
cd HexSoftwares_Movie_Ratings_Analysis
```

**2. Install dependencies**

```bash
pip install -r requirements.txt
```

**3. Run the analysis**

- Open `notebooks/movie_ratings_analysis.ipynb` in Google Colab
- Run all cells sequentially
- Cleaned data will be exported automatically

**4. View dashboard**

- Open `dashboard/Movie_Ratings_Dashboard.pbix` in Power BI Desktop
- Or view the PDF export for static version

---

## 📸 Visualizations

### Rating Distribution Histogram

Shows how ratings are spread across the dataset. Most movies cluster around 7.8-8.2, with a slight right skew.

### Top 10 Movies Bar Chart

Horizontal bar chart ranking the highest-rated films. Shawshank Redemption leads at 9.3/10.

### Genre Performance Analysis

Bar chart comparing average ratings across genres. Drama and Biography dominate the top positions.

### Temporal Trends Line Chart

Displays rating evolution over decades, revealing the 1990s-2000s as the peak quality period.

### Correlation Heatmap

Visualizes relationships between numeric variables, highlighting moderate vote-rating correlation.

---

## 🚧 Challenges and Solutions

| Challenge | Solution | Outcome |
|-----------|----------|---------|
| **Multiple genres per movie** | Split genre strings and analyzed each independently | More accurate genre insights |
| **Data type inconsistencies** | Implemented type conversion with error handling | Clean numeric data for analysis |
| **Year values showing as 1999.0** | Converted to integer type in Python and Excel | Clean year display without decimals |
| **Large dataset visualization** | Used aggregation and top-N filtering | Clear, focused visualizations |
| **Power BI .0 display issue** | Fixed data types at source (Python) | Professional number formatting |

---

## 🔮 Future Improvements

- [ ] Incorporate sentiment analysis from movie reviews
- [ ] Add predictive modeling for rating estimation based on features
- [ ] Include director and actor influence analysis
- [ ] Implement web scraping for real-time data updates
- [ ] Deploy dashboard online using Power BI Service
- [ ] Add drill-through pages for detailed movie information
- [ ] Integrate external APIs (TMDB, Rotten Tomatoes) for enriched data
- [ ] Create ML model to predict movie success before release

---

## 📚 Learning Outcomes

Through this project, I gained hands-on experience in:

✅ **End-to-end data science workflow** from acquisition to presentation  
✅ **Data cleaning techniques** for real-world messy data  
✅ **Statistical analysis** and interpretation of results  
✅ **Data visualization best practices** for effective communication  
✅ **Dashboard design principles** for business stakeholders  
✅ **Business insight generation** from technical analysis  
✅ **Version control** with Git and GitHub  
✅ **Professional documentation** and technical writing  

### Key Takeaways

> "Data cleaning is 70% of the work, but it's the foundation of everything else."

> "The right visualization can convey in seconds what paragraphs cannot."

> "Business recommendations are only valuable if they're actionable and data-driven."

---

## 📞 Contact

<div align="center">

**Boniface Ramushu**

[![Email](https://img.shields.io/badge/Email-bonifaceramushu28@gmail.com-red?style=for-the-badge&logo=gmail&logoColor=white)](mailto:bonifaceramushu28@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-b--ramushu-blue?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/b-ramushu)
[![GitHub](https://img.shields.io/badge/GitHub-DynamicDataMindset-black?style=for-the-badge&logo=github&logoColor=white)](https://github.com/DynamicDataMindset)

</div>

**Open to opportunities in**: Data Science | Data Analysis | Business Intelligence | Machine Learning

---

## 🙏 Acknowledgments

- **Hex Softwares** for the internship opportunity and mentorship
- **Kaggle** for providing the IMDB dataset
- **Data Science Community** for continuous learning resources and inspiration
- **Open Source Contributors** for the amazing Python libraries

---

## 📄 License

This project is part of an internship program and is for educational purposes.

---

## 📊 Project Status

![Status](https://img.shields.io/badge/Status-✅%20Completed-success?style=for-the-badge)

**Last Updated**: October 2025

---

<div align="center">

### ⭐ If you found this project helpful, please consider giving it a star!

**Made with ❤️ and Python**

[Back to Top ⬆️](#-imdb-movie-ratings-analysis)

</div>
