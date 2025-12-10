
# 🎬 IMDb Movie Sales Analysis – Power BI Dashboard

A **Power BI** project that analyzes **IMDb movie sales**, combining **revenue**, **ratings**, **genres**, and **runtime** to uncover what really drives a **movie’s commercial success**.

---

## 📌 Project Overview

This project uses **IMDb movie data** (999 films, 2006–2016) to answer key business questions like:

- Which **genres** generate the **highest revenue**?
- Do **longer movies** earn more?
- Which **directors** consistently deliver **box-office hits**?
- How have movie **earnings changed over time**, especially with the rise of **streaming**?

The result is an interactive **Power BI dashboard** that helps stakeholders quickly explore **trends, correlations, and performance drivers** across the movie industry.

---

## 🎯 Business Objective

The project focuses on turning raw IMDb data into **actionable business insights**:

- Identify **top-performing genres** and **directors** based on **revenue trends**.  
- Analyze **audience engagement** using **IMDb ratings** and **number of votes**.  
- Understand **year-wise shifts** in popularity and market performance.  
- Provide **data-backed recommendations** for studios, producers, and content platforms.

---

## 🧰 Tech Stack

- **Power BI** – data modeling & interactive dashboard  
- **DAX** – calculated columns & measures  
- **Power Query** – data cleaning & transformations  
- **Microsoft Excel / CSV** – source data format  

---

## 🧹 Data Preparation

Key **data preparation** steps performed in **Power Query** / **Power BI**:

- **Imported** the IMDb dataset into **Power BI**.  
- **Handled missing values** in columns like **Revenue (Millions)** and **Metascore**.  
- **Changed data types**:
  - `Revenue (Millions)`, `Metascore` → **Decimal Number**
  - `Year`, `Runtime (Minutes)` → **Whole Number**
- **Cleaned multi-genre fields** by splitting entries such as  
  `Action|Adventure|Sci-Fi` → **Action**, **Adventure**, **Sci-Fi** (for better aggregation).  
- Ensured a **clean star-schema-like model** for smooth visuals and measures.

---

## 📊 Dashboard & Key Visuals

The main dashboard (see `assets/dashboard_preview.png`) contains:

1. **KPI Cards**
   - **Avg Revenue**
   - **Avg Runtime**
   - **Avg IMDb Rating**
   - **Total No. of Movies**

2. **Trend of Genre Revenue Over Time**
   - Line chart showing **genre-wise revenue** from **2006–2016**.  
   - **Action** & **Adventure** peak around **2012–2013**, followed by a **30–40% revenue decline** post-2013.

3. **Distribution of Revenue by Genre**
   - Bar chart ranking genres by **total revenue**.  
   - Highlights **high-earning genres** vs **low-performing ones**.

4. **Highest Revenue by Director**
   - Donut / pie chart showing **share of revenue** contributed by **top directors**.

5. **Movie Count by Genre**
   - Pie chart showing **share of total movies** by genre.  
   - **Drama** dominates volume (~29%), but does not always lead in revenue.

6. **Runtime vs Revenue**
   - Line/area chart showing the relationship between **average runtime** and **revenue**.  
   - Movies around **110–120 minutes** often hit **revenue highs**, but “longer ≠ always better”.

7. **Genres with Highest IMDb Ratings**
   - Bar chart of **max IMDb rating** by genre.  
   - **Biography** and **Sci-Fi** hit **ratings up to 9.0**, while **Horror** and **Thriller** tend to score lower.

---

## 💡 Key Insights

Some of the most important insights:

- **Revenue Peaks (2010–2015)**  
  - **Action**, **Adventure**, and **Animation** films drove major box office success, especially between **2010–2013**.
- **Post-2013 Revenue Drop**  
  - Overall movie earnings **declined after 2013**, likely due to **streaming platforms** disrupting traditional box office.
- **Genre Performance**  
  - **Drama** has the **largest share of movies** but often **underperforms financially**.  
  - **Biography** and **Sci-Fi** are **highly rated** despite smaller volume → strong candidates for **niche, high-impact projects**.
- **Runtime Sweet Spot**  
  - Movies around **110–120 minutes** tend to balance **audience engagement** and **revenue performance**.
- **Director Impact**  
  - A few **top directors** (e.g., high-grossing action/animation experts) account for a **disproportionate share of revenue**, proving the value of **brand-name direction**.

---

## 🏗️ Project Structure

```text
IMDb-Movie-Sales-Analysis-PowerBI/
├── README.md
├── data/
│   └── imdb_movies_raw.csv              # Original dataset
├── pbix/
│   └── IMDb_Movie_Sales_Analysis.pbix   # Main Power BI file
├── reports/
│   └── IMDb_Movie_Sales_Analysis.pdf    # Presentation / documentation
└── assets/
    └── dashboard_preview.png            # Screenshot of final dashboard
```

---

### ✅ Conclusion

The ** IMDb Movie Sales Analysis** highlights how **genre**, **director**, **runtime**, and **audience ratings** collectively shape a movie’s **box-office performance**.  
While **Action** and **Adventure** movies dominated **revenue** during the early 2010s, **Biography** and **Sci-Fi** films achieved some of the **highest audience ratings**, proving that commercial success and critical appreciation do not always overlap.

The dashboard also reveals a noticeable **decline in revenue after 2013**, suggesting the growing influence of **streaming platforms** and changing viewer behavior.  
By transforming raw IMDb data into an interactive **Power BI dashboard** with **DAX-powered insights**, this project demonstrates strong skills in **data cleaning**, **data modeling**, and **storytelling with visuals**, and shows how data can support **smarter decisions** in the movie and entertainment industry.
