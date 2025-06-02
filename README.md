# 🎬 Netflix Insights: Trends & Genres Analysis

This project presents an interactive Tableau dashboard that offers a deep-dive analysis into Netflix's content library. It explores global trends in show releases, genre popularity, and country contributions using a Kaggle dataset.

🔗 **[Live Dashboard on Tableau Public](https://public.tableau.com/app/profile/aditya.kumar6665/viz/GlobalNetflixInsightsTrendsGenres/Visualizations)**  
📦 **Dataset**: [Netflix Shows Dataset - Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)

---

## 📚 Table of Contents

- [📌 Project Highlights](#-project-highlights)
- [🧰 Tools Used](#-tools-used)
- [📊 Dataset Summary](#-dataset-summary)
- [📈 Visualizations & Screenshots](#-visualizations--screenshots)
  - [1. Shows Released Per Year](#1-shows-released-per-year)
  - [2. Content Type Breakdown](#2-content-type-breakdown)
  - [3. Country-Wise Content Contribution](#3-country-wise-content-contribution)
  - [4. Genre Frequency](#4-genre-frequency)
  - [5. Top Directors](#5-top-directors)
  - [6. Top Cast Members](#6-top-cast-members)
  - [7. Duration Breakdown](#7-duration-breakdown)
- [🧠 Key Insights](#-key-insights)
- [📂 Files in Repository](#-files-in-repository)
- [📸 Screenshot Checklist](#-screenshot-checklist-upload-to-screenshots-folder)
- [🚀 How to Run](#-how-to-run)
- [🙏 Acknowledgments](#-acknowledgments)
- [📬 Contact](#-contact)

---

## 📌 Project Highlights

- Analyze release trends of movies and shows over time
- Discover top producing countries and genres
- Number of records by content type
- Distribution of different ratings across all Netflix content
- Built using Tableau Public with custom visuals

---

## 🧰 Tools Used

| Tool     | Role                            |
|----------|----------------------------------|
| Tableau  | Dashboarding, Data Analysis      |
| Excel    | Initial dataset formatting       |
| Kaggle   | Dataset source                   |

---

## 📊 Dataset Summary

- **Source**: Netflix Titles Dataset by Shivam Bansal
- **File**: `netflix_titles.csv`
- **Records**: 8,800+ titles
- **Key Fields**: show_id, type, title, director,	cast,	country, date_added, release_year, rating, duration, listed_in,	description

---

## 📈 Visualizations & Screenshots

### 1. 📅 Shows Released Per Year
- **Chart**: Line Chart  
- **Formula**:
  ```tableau
  COUNT([Title]) BY YEAR([Date Added])
  ```
- **Screenshot**: `/screenshots/shows_by_year.png`

---

### 3. 🌍 Country-Wise Content Contribution
- **Chart**: Bar Chart  
- **Formula**:
  ```tableau
  COUNT([Title]) by [Country]
  ```
- **Screenshot**: `/screenshots/top_countries.png`

---

### 4. 🎭 Distribution of Genre
- **Chart**: Treemaps  
- **Formula**:
  ```tableau
  SPLIT([Listed_in], ",")
  ```
- **Screenshot**: `/screenshots/genre_distribution.png`

---

### 5. 👨‍🎬 Distribution of different Ratings
- **Chart**: Pie Chart  
- **Formula**:
  ```tableau
  COUNT([Title]) by [Ratings]
  ```
- **Screenshot**: `/screenshots/top_directors.png`

---

### 6. 🎭 Distribution of Content Type
- **Chart**: Horizontal Bar  
- **Formula**:
  ```tableau
  COUNT([Title]) by [Type]
  ```
- **Screenshot**: `/screenshots/top_cast.png`

## 🧠 Key Insights

- Netflix scaled rapidly in 2011–2018.
- Dramas and International Movies dominate.
- USA, India, and UK are top contributors.
- Movies reach the world fast; TV shows build loyal fans over time.

---

## 📂 Files in Repository

| File/Folder                    | Description                                |
|--------------------------------|--------------------------------------------|
| `Netflix_Insights.twbx`        | Tableau Packaged Workbook                  |
| `screenshots/`                 | Contains all chart screenshots             |
| `NetflixDataset.csv`           | Optional: cleaned Netflix CSV file         |
| `README.md`                    | Project overview and documentation         |

---

## 🙏 Acknowledgments

- Dataset by [Shivam Bansal on Kaggle](https://www.kaggle.com/shivamb)
- Visualization and design by **Aditya Kumar**

---

## 📬 Contact

- **LinkedIn**: [Aditya Kumar](https://www.linkedin.com/in/aditya-kumar-199b18180)
- **Tableau**: [Public Profile](https://public.tableau.com/app/profile/aditya.kumar6665)

---

> © 2025 Aditya Kumar — Netflix Trends Dashboard
