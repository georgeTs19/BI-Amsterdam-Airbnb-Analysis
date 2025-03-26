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

Download the reviews.csv.gz dataset from the Inside Airbnb website and place it in the datasets folder.

Open the BI-PreProccessingDatasetFINAL.ipynb notebook and run the code to preprocess the datasets.

Use the processed files in a BI application of your choice for further analysis.

Qlik Dashboard Analysis & Insights
This section includes key insights obtained from the Qlik dashboard, categorized into different sheets.

Neighbourhood Dynamics for Hosts
Insights:

Revenue Distribution: The highest revenue is concentrated in central neighbourhoods like De Baarsjes - Oud-West, Centrum-West, and De Pijp - Rivierenbuurt, indicating these areas are Airbnb hotspots.

Room Type Preference: Entire home/apartments dominate the revenue stream, making up 88.1% of total revenue, while private rooms contribute only 10.8%.

Occupancy Rate Trends: Certain neighbourhoods like Bijlmer-Centrum and Bijlmer-Oost have occupancy rates above 70% across all seasons, suggesting strong demand in these areas.

Reviews Analysis
Insights:

Total Reviews: Over 440.8k reviews have been recorded, with an overwhelming 98.62% positive feedback rate.

Best Performing Hosts: Some hosts have exceptionally high review rates, with CityHub having 2907 reviews per listing, indicating a strong and engaged customer base.

Common Positive Feedback: Guests frequently mention great location, perfect stay, and highly recommended, emphasizing the importance of location and hospitality quality.

Neighbourhood Dynamics for Renters
Insights:

Price Variation Across Neighbourhoods: The highest prices are found in Buitenveldert - Zuidas, Centrum-West, and Centrum-Oost, with some listings exceeding €500 per night.

Distance vs. Price Clusters: Listings closer to the city center tend to have higher prices, while neighbourhoods further from the center exhibit more competitive pricing.

Occupancy Rates: Bijlmer-Centrum, Bos en Lommer, and De Baarsjes - Oud-West have the highest occupancy rates, suggesting they are preferred locations due to affordability or proximity to major attractions.

License
This project is licensed under the MIT License. Feel free to use and modify the code as needed.

Project Context
This repository was created as part of a project for the INFN45: Business Intelligence course in the Master’s Programme in Information Systems at Lund University.


