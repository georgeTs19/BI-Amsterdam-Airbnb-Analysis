# BI-Amsterdam-Airbnb-Analysis

An analytical project exploring Airbnb listings in Amsterdam using data from Inside Airbnb, Statista, and other sources. This repository focuses on the preprocessing steps required to prepare the datasets for integration into a business intelligence (BI) application for further analysis.

## Table of Contents
1. [Project Overview](#project-overview)
2. [Contents of the Repository](#contents-of-the-repository)
3. [Preprocessing](#preprocessing)
4. [How to Use](#how-to-use)
5. [Qlik Dashboard Analysis & Insights](#qlik-dashboard-analysis--insights)
   - [Neighbourhood Dynamics for Hosts](#neighbourhood-dynamics-for-hosts)
   - [Reviews Analysis](#reviews-analysis)
   - [Neighbourhood Dynamics for Renters](#neighbourhood-dynamics-for-renters)
6. [License](#license)

---

## Project Overview
This project involves preprocessing raw datasets to clean, structure, and enhance them for analysis. The processed files can be used in BI tools like Qlik Sense to analyze Airbnb pricing, availability, reviews, and tourism trends, as well as compare Airbnb performance with Amsterdam’s hotel market.

## Contents of the Repository
- `datasets/`: Contains the raw datasets required for preprocessing. Refer to the `datasets/README.md` for details about the files.
- `BI-PreProccessingDatasetFINAL.ipynb`: Jupyter Notebook with the full preprocessing pipeline.
- `BI-Amsterdam-Analysis.pdf`: A comprehensive document containing the preprocessing code, results, and insights for users unable to run the code.
- `screenshots/`: Folder containing screenshots of the Qlik dashboard analysis.
- `README.md`: Overview of the preprocessing steps and repository structure.

## Preprocessing
The preprocessing pipeline was implemented in Python using libraries such as `pandas`, `numpy`, and `NLTK`. It focuses on preparing the datasets for seamless integration into BI tools.

### Key Preprocessing Steps:
- **Data Cleaning**: Addressed missing values, removed duplicates, and standardized formats.
- **Feature Engineering**: Created new variables, such as `distance_to_center`, to enhance analytical value.
- **Sentiment Analysis**: Performed sentiment analysis on guest reviews using the VADER lexicon, with filtering for English comments.
- **Reshaping Tourism Data**: Cleaned and reshaped hotel tourism data from Statista into a format suitable for temporal analysis.
- **Outlier Detection and Removal**: Identified and handled outliers in pricing and other numeric fields.

The complete code for these steps is provided in the `BI-PreProccessingDatasetFINAL.ipynb` notebook.

## How to Use
1. Clone this repository:  
   ```bash
   git clone https://github.com/georgeTs19/BI-Amsterdam-Airbnb-Analysis.git
