# Data-Extraction-and-Analysis-on-Anime-TV-Dataset
Complete Data Extraction and Analysis for Beginners

# 📊 Anime Data Analysis

This repository contains a Jupyter notebook (`Anime Code.ipynb`) that performs structured analysis on an anime dataset. The notebook includes steps for data loading, cleaning, feature extraction, and exploration.

---

## 📁 Dataset

The dataset (`anime.csv`) is stored in Google Drive and contains anime titles with embedded metadata such as episode count and duration within the title string.

---

## ✅ Steps Performed in the Notebook

1. **📦 Imported Required Libraries**
   - Utilizes `pandas` for data manipulation and cleaning.

2. **🔗 Mounted Google Drive (Colab Specific)**
   - Accessed the dataset from a Drive path using `drive.mount`.

3. **📥 Loaded the Dataset**
   - Read `anime.csv` into a DataFrame from a Drive location.

4. **🧾 Explored the Dataset**
   - Previewed the full DataFrame.
   - Used `df.describe()` to view summary statistics.

5. **🔍 Accessed Specific Records**
   - Retrieved individual titles or cell values using `.loc[]` indexing.

6. **🎬 Extracted Episode Count**
   - Used regular expressions on the `Title` column to extract the number of episodes.
   - Created a new column: `No. of Episode`.
   - Handled missing values and converted this column to integer format.

7. **⏱️ Extracted Duration**
   - Applied regex to extract the episode duration from titles (e.g., `24 min`).
   - Created a new column: `Duration`.
   - Cleaned and converted the duration to numeric (in minutes) for analysis.

8. **🧪 Verified Data Types**
   - Used `df.dtypes` to confirm the structure after transformations.

---

## 🛠️ Requirements

To run the notebook:

```bash
python>=3.8
google colab
pandas
