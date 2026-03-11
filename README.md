# 🎬 Movie Industry Data Analysis (Python Project)

## 📌 Project Overview

This project analyzes a large dataset of movies to discover **what factors influence movie revenue and profitability**.

Using **Python, Pandas, Matplotlib, and Seaborn**, we performed data cleaning, feature engineering, correlation analysis, and data visualization to uncover insights about the movie industry.

The goal is to identify patterns between variables such as **budget, votes, genre, and revenue** and understand which elements drive financial success in films.

---

# 🎯 Business Problem

Movie studios invest millions in film production but often lack clear insights into **what factors contribute most to box office success**.

### Key Questions

* Does a **higher budget** lead to higher revenue?
* Do **popular movies (votes)** generate more revenue?
* Which **genres** deliver the highest ROI?
* Which **companies and directors** produce the most profitable movies?

---

# 📊 Dataset

The dataset contains information about **5,000+ movies**, including:

* Movie name
* Genre
* Rating
* Release year
* Budget
* Gross revenue
* Votes
* Director
* Production company
* Runtime

Example columns:

| Column  | Description              |
| ------- | ------------------------ |
| name    | Movie title              |
| genre   | Movie genre              |
| year    | Release year             |
| budget  | Movie production budget  |
| gross   | Total box office revenue |
| votes   | Number of user votes     |
| runtime | Movie duration           |

---

# 🛠️ Technologies Used

* **Python**
* **Pandas**
* **Matplotlib**
* **Seaborn**
* **Jupyter Notebook**

---

# 🧹 Data Cleaning

Steps performed to prepare the data:

1. Standardized column names (lowercase + underscores)
2. Converted numeric-like fields (budget, gross, votes) to numeric format
3. Removed rows with missing values
4. Removed duplicate records
5. Reset dataset index
6. Standardized categorical labels (e.g., *Unrated → Not Rated*)

---

# ⚙️ Feature Engineering

Two important business metrics were created:

### ROI (Return on Investment)

```
ROI = (Gross - Budget) / Budget * 100
```

### Profit

```
Profit = Gross - Budget
```

These metrics help evaluate **movie financial performance**.

---

# 🔍 Correlation Analysis

A correlation matrix was generated to examine relationships between numerical variables.

### Strongest Correlations

| Variable 1 | Variable 2 | Correlation |
| ---------- | ---------- | ----------- |
| Gross      | Profit     | 0.98        |
| Budget     | Gross      | 0.74        |
| Votes      | Gross      | 0.61        |
| Budget     | Profit     | 0.61        |

📌 Key Insight
Higher budgets and higher audience engagement (**votes**) tend to correlate with higher revenue.

---

# 📈 Data Visualizations

### Budget vs Gross Revenue

Shows a **strong positive relationship** between movie budget and revenue.

### Votes vs Gross Revenue

Movies with more audience votes generally generate **higher box office revenue**.

### Total Gross by Year

Displays the **trend of total movie revenue over time**.

---

# 📊 Key Insights

### 🎬 Top Movies by Revenue

| Movie                        | Gross Revenue |
| ---------------------------- | ------------- |
| Avatar                       | $2.84B        |
| Avengers: Endgame            | $2.79B        |
| Titanic                      | $2.20B        |
| Star Wars: The Force Awakens | $2.06B        |
| Avengers: Infinity War       | $2.04B        |

---

### 🏢 Top Production Companies by Total Revenue

| Company               | Total Gross |
| --------------------- | ----------- |
| Warner Bros.          | $54B        |
| Universal Pictures    | $51B        |
| Columbia Pictures     | $42B        |
| Paramount Pictures    | $40B        |
| Twentieth Century Fox | $39B        |

---

### 🎭 Genres with Highest ROI

| Genre     | Average ROI |
| --------- | ----------- |
| Horror    | 7667%       |
| Family    | 2013%       |
| Thriller  | 329%        |
| Animation | 297%        |
| Drama     | 270%        |

📌 Insight:
Low-budget genres like **Horror** often generate extremely high returns.

---

### 🎥 Most Profitable Directors

| Director      | Movie             | Profit |
| ------------- | ----------------- | ------ |
| James Cameron | Avatar            | $2.61B |
| Anthony Russo | Avengers: Endgame | $2.44B |
| James Cameron | Titanic           | $2.00B |
| J.J. Abrams   | Star Wars VII     | $1.82B |

---

# 📌 Summary Statistics

* Total Movies: **5,421**
* Unique Genres: **15**
* Average Budget: **$36M**
* Average Gross Revenue: **$103M**
* Average ROI: **572%**

Strongest correlation:
**Gross vs Profit (98.4%)**

---

# 🚀 Project Structure

```
movie-analysis-project
│
├── movies.csv
├── movie_analysis.ipynb
├── README.md
```

---

# 📈 Business Value

This analysis helps studios and investors:

* Identify **high-performing genres**
* Understand the **impact of budgets**
* Detect **top-performing production companies**
* Predict factors that lead to **box office success**


