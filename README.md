# Netflix Dataset Exploratory Data Analysis (EDA) & Movie Recommendation System

## 📌 Project Overview

This project focuses on **Exploratory Data Analysis (EDA)** of the **Netflix dataset**, uncovering insights about content distribution, genres, directors, and more.
Additionally, a **content-based recommendation system** is implemented using **TF-IDF Vectorization** and **Cosine Similarity** to suggest movies/TV shows based on user input.

---

## 🔧 Technologies Used

* **Python**
* **Libraries**:

  * `pandas`, `numpy` (Data Handling)
  * `matplotlib`, `seaborn` (Data Visualization)
  * `scikit-learn` (TF-IDF & Similarity)

---

## 📂 Dataset

The dataset used is `netflix.csv` containing:

* Show details (title, type, director, cast, country, release year, rating, duration, genres, description)
* ~8800 rows and 12 columns

---

## 📊 Exploratory Data Analysis (EDA)

1. **Content Types on Netflix**

   * Movies: 6126
   * TV Shows: 2664
   * Observation: Netflix has more Movies than TV Shows.

2. **Distribution of Release Years**

   * Most content released between **2000–2020**
   * Peak: **2018** with 1146 releases

3. **Top 10 Countries with Highest Content**

   * United States, India, United Kingdom, Japan, South Korea, etc.

4. **Insights Extracted**

   * TV Shows from India: *79 titles*
   * Movies from India: *893 titles*
   * Top Directors: Rajiv Chilaka, Martin Scorsese, Jay Karas, etc.
   * Genres: 42 unique genres, with *International Movies* and *Dramas* being dominant

---

## 🎬 Movie Recommendation System

A **content-based recommender system** was built with the following steps:

1. **Preprocessing**

   * Selected features: `title`, `director`, `cast`, `listed_in`, `description`
   * Created combined metadata with top actors, director, and genre

2. **Vectorization & Similarity**

   * Applied **TF-IDF Vectorization**
   * Measured similarity using **Cosine Similarity**

3. **User Query Example**

   ```
   Enter a movie/series title: Goodfellas
   ```

   **Top Recommendations:**

   * The Irishman
   * Raging Bull
   * Mean Streets
   * Once Upon a Time in America
   * Midnight Run

---

## 📈 Visualizations

* Count of Movies vs. TV Shows
* Distribution of Release Years
* Top 10 Countries by Content
* Top 10 Genres with Most Content

(All plots are included in the notebook/script.)

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/netflix-eda-recommender.git
   cd netflix-eda-recommender
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the analysis:

   * Open Jupyter Notebook / VS Code and run the EDA script.

4. Run the recommender system:

   ```bash
   python recommender.py
   ```

---

## 📌 Future Work

* Deploy recommender system as a **web app** (Flask/Streamlit)
* Add **collaborative filtering** for better recommendations
* Incorporate **trending analysis** of genres over time

---

## 📜 License

This project is for **educational purposes only**. Dataset is sourced from public repositories.

---



