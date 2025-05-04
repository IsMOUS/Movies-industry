# 🎬 TMDB Movies Dataset Analysis

> *"I always wondered: What makes a movie successful? Is it the cast, the director, the genre… or simply the budget?"*

Driven by this curiosity, I explored a dataset of over 10,000 movies from **TMDB (The Movie Database)** to uncover what drives popularity and financial success in films. From genres and budgets to ratings and revenue, this analysis dives into decades of movie history — from the 1960s to 2015.

---

## 📦 Dataset Overview

This dataset contains detailed information about 10,866 movies, including:

- **Release year**
- **Budget & revenue**
- **Cast, director, and genres**
- **User ratings, popularity scores, and more**

After cleaning and wrangling, I worked with **10,840 clean records**, removing nulls, duplicates, and unnecessary columns to focus on the most meaningful features.

---

## ❓ Key Questions Explored

1. **Do popular movies actually make more money?**
2. **Which genres are most frequently produced?**
3. **Is there a relationship between a movie's budget and its revenue?**

---

## 🧹 Data Preparation Highlights

- Removed duplicates and irrelevant columns.
- Cleaned missing data (notably in `cast`, `director`, and `homepage`).
- Converted `release_date` to datetime format.
- Split multi-entry fields (e.g. `genres`, `cast`) separated by `|`.
- Created new columns:
  - `profit = revenue - budget`
  - Categorized `vote_average` and `profit` into bins for better visualization.

---

## 📊 Key Insights

### 1️⃣ Do popular movies make more revenue?
> ✅ Yes! There's a clear positive trend — the more popular a movie is, the more revenue it tends to generate.

### 2️⃣ What are the most common genres?
> 🎭 `Drama`, 😂 `Comedy`, and 🎬 `Action` are the top 3 genres.  
> Alone, **Drama** appears in over **22%** of the movies.

### 3️⃣ Is there a correlation between budget and revenue?
> 💰 Absolutely. There is a **strong positive correlation** — higher budgets often lead to higher revenue (with a few outliers).

---

## 🛠 Built With

- **Python 3**
- **Jupyter Notebook**
- **Pandas**
- **NumPy**
- **Matplotlib & Seaborn**

---

## 📁 Files in This Repo

- `TMDB_Movie_Analysis.ipynb` — Main analysis notebook
- `tmdb-movies.csv` — Cleaned dataset used
- `TMDB_Report.pdf` — Summary of results (optional for GitHub preview)

---

## 👀 Curious Takeaway

As a movie lover and data enthusiast, this project helped me discover how **data can tell powerful stories**. From budgets and cast to audience votes, every element leaves a trace — and when combined, they reveal fascinating insights into what makes a film succeed.

