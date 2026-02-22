# Netflix Movies & TV Shows Dashboard (Power BI)

## 📊 Project Overview

This project explores Netflix Movies and TV Shows data using Power BI.
The workflow involved extensive data cleaning in Power Query followed by building an interactive dashboard to uncover trends in release years, genres, ratings, and production countries.

---

## 🧹 Data Cleaning & Preparation (Power Query)

The raw CSV required significant preprocessing:

* Fixed malformed CSV row that incorrectly created a new record with “William Wyler” as type
* Handled missing director values by encoding them as "N/A" after exploratory co-actor checks
* Imputed missing country values using mode (United States) as a reasonable assumption
* Created a new feature: movie duration in minutes (null for TV shows)
* Split multi-category genre column into separate rows for accurate aggregation
* Performed simple text-based sentiment classification using keywords (kill, death, murder) to tag Murder Mystery content

---

## 📈 Dashboard Visualizations

### Area Chart

TV Shows vs Movies by Release Year
→ Shows became more popular after 2015, peaking around 2020, while movie releases peaked around 2017.

### Treemap

Top 10 Production Countries
→ United States, United Kingdom, and India dominate Netflix content production.

### Genre Distribution (Horizontal Bar Chart)

→ Most common genre: Documentaries (353 titles)

### Ratings Distribution (Horizontal Bar Chart)

→ Most frequent rating: TV-MA (~3.1K titles)

### Content Type Split (Pie Chart)

→ Movies: ~68%
→ TV Shows: ~32%

### KPI Cards

* Average Movie Duration: 98.28 minutes
* Total Production Countries: 728
* Unique Ratings: 18
* Unique Genres: 468
* Total Titles: 8,278

---

## 🔍 Key Insights

* TV Shows experienced rapid growth after 2015, surpassing movies by 2020
* The US, UK, and India are the largest contributors to Netflix content
* Documentaries are the most frequent genre on the platform
* Mature content (TV-MA) dominates Netflix’s catalog
* Movies still form the majority of Netflix titles (~68%)

---

## 🛠 Tools & Technologies

* Power BI
* Power Query (ETL & Data Cleaning)
* Data Visualization & Dashboard Design
* Basic Text/Sentiment Feature Engineering

---

## 📁 Repository Structure

* `data/` → Raw and cleaned datasets
* `dashboard/` → Power BI (.pbix) file
* `images/` → Dashboard preview screenshots

