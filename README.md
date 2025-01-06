# BI-Amsterdam-Airbnb-Analysis

An analytical project exploring Airbnb listings in Amsterdam using data from Inside Airbnb, Statista, and other sources. This repository focuses on the preprocessing steps required to prepare the datasets for integration into a business intelligence (BI) application for further analysis.

This project was conducted as part of a group assignment for the **INFN45: Business Intelligence** course in the **Master’s Programme in Information Systems at Lund University**.

---

## Project Overview

This project involves preprocessing raw datasets to clean, structure, and enhance them for analysis. The processed files can be used in BI tools like Qlik Sense to analyze Airbnb pricing, availability, reviews, and tourism trends, as well as compare Airbnb performance with Amsterdam’s hotel market.

---

## Contents of the Repository

- **datasets/**: Contains the raw datasets required for preprocessing. Refer to the `datasets/README.md` for details about the files.
- **BI-PreProccessingDatasetFINAL.ipynb**: Jupyter Notebook with the full preprocessing pipeline.
- **BI-Amsterdam-Analysis.pdf**: A comprehensive document containing the preprocessing code, results, and insights for users unable to run the code.
- **README.md**: Overview of the preprocessing steps and repository structure.

---

## Preprocessing

The preprocessing pipeline was implemented in Python using libraries such as pandas, numpy, and NLTK. It focuses on preparing the datasets for seamless integration into BI tools.

### Key Preprocessing Steps:
1. **Data Cleaning**: Addressed missing values, removed duplicates, and standardized formats.
2. **Feature Engineering**: Created new variables, such as `distance_to_center`, to enhance analytical value.
3. **Sentiment Analysis**: Performed sentiment analysis on guest reviews using the VADER lexicon, with filtering for English comments.
4. **Reshaping Tourism Data**: Cleaned and reshaped hotel tourism data from Statista into a format suitable for temporal analysis.
5. **Outlier Detection and Removal**: Identified and handled outliers in pricing and other numeric fields.

The complete code for these steps is provided in the **BI-PreProccessingDatasetFINAL.ipynb** notebook.

---

## How to Use

1. Clone this repository:
git clone https://github.com/georgeTs19/BI-Amsterdam-Airbnb-Analysis.git

2. Download the `reviews.csv.gz` dataset from the [Inside Airbnb website](https://insideairbnb.com/get-the-data/) and place it in the `datasets` folder.
3. Open the **BI-PreProccessingDatasetFINAL.ipynb** notebook and run the code to preprocess the datasets.
4. Use the processed files in a BI application of your choice for further analysis.

---

## License

This project is licensed under the MIT License. Feel free to use and modify the code as needed.

---

## Group Members

This repository was created as part of a group project for the **INFN45: Business Intelligence** course in the **Master’s Programme in Information Systems at Lund University**. 

**Group Members:**
- Alma Magnusson
- Georgios Tsoupras
- Nina Ivarsson

For any questions or feedback, feel free to open an issue in the repository.

