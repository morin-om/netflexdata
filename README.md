# 🎬 Netflix Data Analysis

Exploratory Data Analysis (EDA) of a Netflix movies dataset — uncovering trends in genres, popularity, and release patterns using Python, Pandas, and Plotly.

---

## 📋 Project Overview

This project performs a full end-to-end EDA on a Netflix movies dataset containing **9,826 movies** across **9 features**. The goal is to explore what kinds of content Netflix offers, which genres dominate, which movies are most popular, and how content production has grown over time.

---

## 📁 Dataset

**File:** `NetflixData.csv`

| Column | Description |
|--------|-------------|
| `Release_Date` | Date the movie was released |
| `Title` | Movie title |
| `Overview` | Short description of the movie |
| `Popularity` | Popularity score from TMDB |
| `Vote_Count` | Number of votes received |
| `Vote_Average` | Average user rating (0–10) |
| `Original_Language` | Language the movie was made in |
| `Genre` | Genre(s) of the movie |
| `Poster_Url` | Link to the movie poster image |

---

## 🔍 Analysis Steps

**1. Data Loading & Preview** — Load the CSV and inspect the first few rows and shape.

**2. Dataset Structure** — Check columns, data types, and memory usage.

**3. Statistical Summary** — Describe numerical columns (Popularity, Vote Count, Vote Average).

**4. Data Quality Check** — Identify duplicate rows (2 found) and missing values.

**5. Data Cleaning** — Remove duplicates and drop rows with null values. Final clean dataset: **9,821 rows**.

**6. Data Preprocessing** — Convert `Release_Date` to datetime and extract the release year. Drop irrelevant columns (`Overview`, `Poster_Url`, `Original_Language`). Explode multi-genre rows so each genre gets its own row → final shape: **25,779 rows × 6 columns**.

**7. Data Visualization** — Four interactive charts built with Plotly Express:
- Most common genres (bar chart)
- Top 10 most popular movies (horizontal bar chart)
- Movies released over the years (line chart)
- Distribution of popularity scores (histogram)

---

## 📊 Key Findings

- **Drama** is the most frequently occurring genre on Netflix, followed by Comedy and Action.
- **Spider-Man: No Way Home** has the highest popularity score in the dataset, followed by The Batman and Encanto.
- **Movie production has grown steadily**, especially after 2000, with 2019 seeing the highest number of releases in the dataset.
- **Adventure** movies have the highest average popularity score, followed by Action and Animation.
- **Popularity is heavily right-skewed** — most movies are average, while only a handful become major hits.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas | Data loading, cleaning & transformation |
| Plotly Express | Interactive visualizations |
| Google Colab | Development environment |

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/netflix-data-analysis.git
   cd netflix-data-analysis
   ```

2. Install dependencies:
   ```bash
   pip install pandas plotly
   ```

3. Add `NetflixData.csv` to the project folder.

4. Open and run `Netflix_Data_Analysis.ipynb` in Jupyter or Google Colab.

---

## 📂 Repository Structure

```
netflix-data-analysis/
├── Netflix_Data_Analysis.ipynb   # Main analysis notebook
├── NetflixData.csv               # Dataset (add manually)
└── README.md                     # Project documentation
```

---

## 📌 Dataset Source

Data sourced from [Kaggle — Netflix Movies and TV Shows](https://www.kaggle.com/datasets/shivamb/netflix-shows). Metadata powered by TMDB.

---

*Built with Python & Plotly | EDA Project*
