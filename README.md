# 🎬 CineInsights: Exploring the TMDB 5000 Movies Dataset 📊

![Movie Analysis Banner](https://img.shields.io/badge/Movie%20Analysis-Data%20Science-brightgreen)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Kaggle](https://img.shields.io/badge/Kaggle-Dataset-orange)

## 📝 Project Overview

Welcome to **CineInsights** - a comprehensive exploratory data analysis of the TMDB 5000 Movies Dataset! This project dives deep into the fascinating world of cinema, uncovering patterns, trends, and insights about what makes movies successful. Through statistical analysis and visualizations, we answer 12 key questions about movie revenue, ratings, genres, directors, and more.

## 🔍 Dataset

The analysis is performed on the TMDB 5000 Movies Dataset, which contains detailed information on 4803 movies including their budget, revenue, genres, ratings, and other attributes.

🔗 **[Dataset Link on Kaggle](https://www.kaggle.com/datasets/akshaydattatraykhare/movies-dataset/data)**

## 🛠️ Tools & Libraries Used

- **Python** 📊
- **Pandas** 🐼
- **NumPy** 🔢
- **Matplotlib** 📈
- **Seaborn** 🎨
- **Scikit-learn** 🧠

## 🧹 Data Preprocessing Steps

1. **Data Cleaning** 🧼
   - Converted JSON strings into lists/dictionaries for genres, keywords, production companies, etc.
   - Replaced infinite values with NaN
   - Extracted genre names into a separate column
   - Filled missing values in tagline with empty strings

2. **Feature Engineering** ⚙️
   - Converted release dates to datetime format
   - Created new columns for release year and month
   - Computed number of spoken languages
   - Converted revenue to millions
   - Created binary indicator for English movies
   - Calculated Return on Investment (ROI) percentage
   - Measured tagline length

3. **Missing Value Handling** 🔍
   - Dropped homepage column due to significant missing values
   - Removed row with missing release date
   - Imputed missing overview values with empty strings

## 📊 Statistical Analysis

### Correlation Analysis 📉
- **Pearson Correlation**: Measured linear relationships between numerical variables
  - Found strong positive correlation (0.78) between popularity and vote count
  - High correlation (0.73) between revenue and budget
  - Good positive correlation (0.64) between revenue and popularity

- **Spearman Correlation**: Assessed monotonic relationships (rank-based)
  - Revealed strong correlation (0.76) between revenue and budget
  - Extremely strong correlation (0.96) between popularity and vote count
  - All financial metrics strongly correlated with each other

### Partial & Semi-Partial Correlation 🔬
- Analyzed vote average and revenue while controlling for budget (r = 0.293)
- Performed semi-partial correlation analysis (r = 0.2466)

### Normality Tests 📏
- **Kolmogorov-Smirnov (KS) Test**: Indicated data is not normally distributed
- **Anderson-Darling Test**: Confirmed non-normality in the dataset
- **Q-Q Plots**: Visualized deviations from normality for all numerical features
  - Most features exhibit strong right or left skewness
  - Some features follow S-shaped distributions
- **Distribution Plots**: Created distribution plots of all numerical features

## 🔎 Research Questions & Findings

### 1️⃣ What genres of movies have the highest average revenue?
- Animation, Adventure, and Fantasy genres have the highest average revenue
- Documentary genre has the highest ROI (over 250%)
- Drama is the most common genre (present in 2297 movies)

### 2️⃣ Is there a correlation between movie budgets and Ratings?
- No strong correlation exists between movie budgets and ratings
- High budget doesn't guarantee high ratings

### 3️⃣ Which directors have consistently high box office success?
- **Revenue Kings**: Steven Spielberg, Peter Jackson, James Cameron
- **ROI Masters**: Pierre Coffin, George Lucas, James Cameron
- **Consistently Successful**: James Cameron, Christopher Nolan, Ridley Scott, Peter Jackson
- Christopher Nolan and James Cameron show the greatest career growth trend

### 4️⃣ How do user ratings compare between movies in the same genre but different production years?
- Overall rating decline from 1920 to 2020
- Films from 1930-1950 have higher ratings on average
- Animation has highest median rating; Horror has lowest
- Drama maintains the most consistent ratings over time

### 5️⃣ How has the average movie budget changed over time?
- Sharp budget increase around 1925 (silent to talking films transition)
- Steady upward trend since 1980
- Science Fiction, Fantasy, Adventure, and Animation have highest recent budgets
- Horror consistently maintains low budgets

### 6️⃣ Which months are most popular for movie releases?
- September has highest number of releases (film festival season)
- December is second-highest (holiday & Oscar-qualifying season)
- June/July show strong numbers (summer blockbuster season)
- Monthly releases increased dramatically from 0-5 (1920s-1970s) to 15-40 (2000s-2010s)

### 7️⃣ How does the number of spoken languages correlate with international revenue?
- Movies with 4-6 languages show higher median revenues
- Action, Adventure, and Sci-Fi films with multiple languages perform best
- 4-6 languages appears to be the "sweet spot" for maximizing revenue

### 8️⃣ What's the distribution of movie runtimes by genre?
- Most movies fall between 90-120 minutes
- Animation and Family films are shortest (around 90 minutes)
- History, War, and Crime genres have longest runtimes
- Higher-revenue films tend to have longer runtimes
- Runtimes have stabilized since the 1980s between 90-110 minutes

### 9️⃣ Is there a trend in movie popularity over the years?
- Significant popularity spikes around 1940, 1960, and 2015-2018
- 2010s show dramatic upward trend in popularity
- Movies with more languages achieve higher popularity
- 1937, 2014, and 2015 were standout years for movie popularity

### 🔟 How do production countries affect global revenue?
- US dominates global movie revenue and production volume
- Smaller countries like Dominica and Jamaica show higher average revenue per film
- All countries show revenue growth since 1990s-2000s
- Japan shows exceptional revenue spike around 2015-2020

### 1️⃣1️⃣ What's the ROI (Return on Investment) distribution across genres?
- Documentary and Music genres have highest median ROI
- Horror films offer high returns on relatively low budgets
- Japan has highest median ROI among countries
- ROI volatility has decreased since the 1980s

### 1️⃣2️⃣ Is there a correlation between movie tagline length and popularity?
- Medium-length taglines (10-60 characters) correlate with highest popularity
- Weak negative correlation between tagline length and popularity
- Short taglines have the lowest median popularity

## 🚀 How to Use This Repository

1. Clone the repository:
```bash
git clone https://github.com/yourusername/CineInsights.git
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

3. Open the Jupyter Notebook:
```bash
jupyter notebook TMDB_Movie_Analysis.ipynb
```


## 👨‍💻 Author

Mayank Mittal

---

⭐ If you find this project interesting, please consider giving it a star! ⭐
