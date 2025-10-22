# VOIS_AICTE_Oct2025_MajorProject_SydelWivelAfonso
# 🎬 Netflix Dataset Analysis — Insights from 7,789 Titles

## 📖 Overview  
This project explores the **Netflix Dataset** containing over **7,700 movies and TV shows**, uncovering patterns in content type, release years, genres, countries, and ratings.  
Using **Python (Pandas, Matplotlib, Seaborn)**, this analysis aims to understand Netflix’s content strategy, regional preferences, and the evolution of its catalog over time.

---

## 🧩 Key Objectives  
- 🔍 Understand the distribution between **Movies and TV Shows**  
- 📅 Analyze **content trends over the years**  
- 🌍 Identify **top countries** contributing Netflix titles  
- 🎭 Discover **most popular genres**  
- 🎞️ Examine **content ratings** (e.g., TV-MA, TV-14, PG)  

---

## 🧠 Dataset Information  

| Attribute | Description |
|------------|-------------|
| **Show_Id** | Unique ID for each title |
| **Category** | Type of content – Movie or TV Show |
| **Title** | Name of the movie or show |
| **Director** | Director name(s) |
| **Cast** | Cast members |
| **Country** | Country of production |
| **Release_Date** | Date added to Netflix |
| **Rating** | Audience rating (TV-MA, PG, etc.) |
| **Duration** | Runtime for movies or number of seasons for shows |
| **Type** | Genre categories |
| **Description** | Short synopsis of the title |

📊 **Total Records:** 7,789  
🧼 **Data Cleaning:** Missing values handled (`Unknown` filled), and release dates converted to datetime.

---

## ⚙️ Technologies Used  
- 🐍 **Python 3**  
- 📘 **Pandas** – Data manipulation  
- 📊 **Matplotlib & Seaborn** – Visualization  
- ☁️ **Google Colab** – Execution environment  

---

## 📈 Visual Insights  

### 🎥 Content Type Distribution  
Netflix hosts **more Movies than TV Shows**, showing a higher investment in film content.

### 📅 Yearly Trend  
A rapid increase in content addition was seen **between 2017–2020**, marking Netflix’s global expansion phase.

### 🎭 Top 10 Genres  
- **Dramas**, **Comedies**, and **Documentaries** dominate the platform.  
- Reflects Netflix’s focus on storytelling and cultural diversity.

### 🌍 Top Countries  
| Rank | Country | Flag |
|------|----------|------|
| 1️⃣ | United States | 🇺🇸 |
| 2️⃣ | India | 🇮🇳 |
| 3️⃣ | United Kingdom | 🇬🇧 |
| 4️⃣ | Canada | 🇨🇦 |
| 5️⃣ | France | 🇫🇷 |

The **U.S. leads** in total content produced for Netflix.

### 🔢 Content Ratings  
- **TV-MA** and **TV-14** are the most frequent ratings.  
- Suggests that **mature and teen audiences** are Netflix’s largest demographics.

---

## 🧮 Sample Visualizations  

| Insight | Visualization |
|----------|----------------|
| Content Distribution | `sns.countplot(x='Category')` |
| Yearly Trend | `df.groupby(['year_added','Category']).size().unstack()` |
| Top Genres | `sns.barplot(y='Genre', x='Count')` |
| Top Countries | `sns.barplot(y=country_df.index, x=country_df.values)` |
| Ratings Distribution | `sns.countplot(x='Rating')` |

---

## 💡 Summary Insights  
✅ **Movies dominate** Netflix’s library  
📆 **Content surged** between *2017–2020*  
🎭 **Top genres:** Drama, Comedy, Documentary  
🌍 **USA, India, UK** — Top 3 contributors  
🔞 **TV-MA and TV-14** — Most common ratings  

---

## 🚀 How to Run  

1. Mount Google Drive in Colab  
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
