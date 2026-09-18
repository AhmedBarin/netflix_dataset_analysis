# 📊 Netflix Dataset Analysis

| Field        | Details                          |
|-------------|----------------------------------|
| **Date**     | March 2026                     |
| **Status**   | ✅ Completed                       |
| **Role**     | AI Engineer                      |
| **Tech Stack** | Python, Pandas, NumPy, Matplotlib, Seaborn |

---

## Overview

An exploratory data analysis (EDA) of the Netflix Shows & Movies dataset (8,807 titles, 12 columns). The project investigates content trends across countries, genres, ratings, and release years — revealing how the streaming landscape evolved and how global events like the pandemic impacted content production.

## Key Questions Answered

| # | Question | Visualization |
|---|----------|---------------|
| Q1 | Top 10 movie-producing countries? | Bar chart |
| Q2 | Top 10 TV show-producing countries? | Bar chart |
| Q3 | TV show duration distribution? | Histogram |
| Q4 | Movie duration distribution? | Histogram |
| Q5 | Movies vs. TV shows split? | Count plot |
| Q6 | Content added year-by-year trend? | Line chart |
| Q7 | Pandemic impact on content production? | Line chart (2020 dip) |
| Q8 | Top countries for kids' content? | Pie chart |
| Q9 | Most productive directors? | Bar chart |
| Q10 | Top 10 genres on Netflix? | Horizontal bar chart |
| Q11 | Content added by month? | Count plot |
| Q12 | Content ratings distribution? | Count plot |
| Q13 | Egyptian content breakdown? | Type split chart |

## Architecture

```
Raw Data (netflix_titles.csv)
        │ 8,807 titles × 12 columns
        ▼
┌───────────────┐
│  Data Loading  │  ← pd.read_csv(), df.info(), head()
└───────┬───────┘
        │
        ▼
┌───────────────┐
│  Missing Data  │  ← Fill NaN with 'Unknown' or mode
│  Cleaning      │     (director, cast, country, rating, etc.)
└───────┬───────┘
        │
        ▼
┌───────────────┐
│  EDA & Visuals │  ← 13 analysis questions with
│                │     bar charts, histograms, pie charts, line plots
└───────────────┘
```

## Key Findings

- **Content Growth:** Netflix content surged significantly starting around 2010, with a notable dip in 2020 likely due to the COVID-19 pandemic.
- **Country Dominance:** The United States leads both movie and TV show production, followed by India and the United Kingdom.
- **Genre Popularity:** Dramas dominate as the most common genre across Netflix's catalog.
- **Egyptian Content:** 117 titles are produced in Egypt, with a notable split between movies and TV shows.
- **Kids' Content:** The US leads children's content production, followed by India and the UK.

## Repository Structure

```text
ML college project netflix dataset analysis/
├── netflix_titles.csv              # Dataset (Kaggle: Netflix Shows)
└── netflix_dataset_analysis.ipynb  # Full EDA with 13 visualizations
```

> **Note:** Uses the public Kaggle "Netflix Shows & Movies" dataset by Shivamb. No external API keys or credentials required.
