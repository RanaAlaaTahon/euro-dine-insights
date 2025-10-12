# **EuroDine Insights**

**EuroDine Insights** is a data analysis project based on the [TripAdvisor Restaurants Info for 31 Euro-Cities Dataset](https://www.kaggle.com/datasets/damienbeneschi/krakow-ta-restaurans-data-raw/data)
, featuring over 125,000 restaurants across 31 European cities. Using Python-based analytical and visualization tools, the project explores customer ratings, cuisine preferences, and regional dining trends, through statistical testing.

## Table of Contents

<details>
  <summary>Click here to expand the contents</summary>

- [Project Outcomes and Key Findings](#project-outcomes-and-key-findings)
- [Dataset Content](#dataset-content)
- [Business Requirements](#business-requirements)
- [Hypothesis and Validation](#hypothesis-and-validation)
- [Project Plan](#project-plan)
- [The rationale to map the business requirements to the data visualizations](#-the-rationale-to-map-the-business-requirements-to-the-data-visualizations)
- [Analysis Techniques Used](#analysis-techniques-used)
- [Ethical Considerations](#ethical-considerations)
- [Dashboard Design](#dashboard-design)
- [Wireframe](#wireframe)
- [Tableau Dashboard](#tableau-dashboard)
- [Kanban Board](#kanban-board)
- [Unfixed Bugs](#unfixed-bugs)
- [Development Roadmap](#development-roadmap)
- [Main Data Analysis Libraries](#main-data-analysis-libraries)
- [Credits](#credits)

</details>

## Project Outcomes and Key Findings

-
-
-
-

## Dataset Content

- [TripAdvisor Restaurants Info for 31 Euro-Cities Dataset](https://www.kaggle.com/datasets/damienbeneschi/krakow-ta-restaurans-data-raw/data)

* The dataset contain restaurants information for 31 cities in Europe: Amsterdam (NL), Athens (GR) , Barcelona (ES) , Berlin (DE), Bratislava (SK), Bruxelles (BE), Budapest (HU), Copenhagen (DK), Dublin (IE), Edinburgh (UK), Geneva (CH), Helsinki (FI), Hamburg (DE), Krakow (PL), Lisbon (PT), Ljubljana (SI), London (UK), Luxembourg (LU), Madrid (ES), Lyon (FR), Milan (IT), Munich (DE), Oporto (PT), Oslo (NO), Paris (FR), Prague (CZ), Rome (IT), Stockholm (SE), Vienna (AT), Warsaw (PL), Zurich (CH).

* The data is a .csv file comma-separated that contains 125 433 entries (restaurants). It is structured as follow:

| Column                | Description                                                                                                             |
| --------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **Name**              | Name of the restaurant                                                                                                  |
| **City**              | City where the restaurant is located                                                                                    |
| **Cuisine Style**     | Cuisine style(s) of the restaurant, stored as a Python list                                                             |
| **Ranking**           | Rank of the restaurant among all restaurants in the city (float)                                                        |
| **Rating**            | Customer rating of the restaurant on a scale from 1 to 5 (float)                                                        |
| **Price Range**       | Price category of the restaurant among 3 categories (categorical)                                                       |
| **Number of Reviews** | Total number of customer reviews (float)                                                                                |
| **Reviews**           | Two sample reviews with their dates, stored as a list of lists: first list contains reviews, second list contains dates |
| **URL_TA**            | Part of the TripAdvisor URL for the restaurant page, after 'www.tripadvisor.com' (string)                               |
| **ID_TA**             | Unique identifier of the restaurant in the TripAdvisor database (one letter + number)                                   |

## Business Requirements

The primary goal of this project is to translate business requirements into actionable insights through intuitive and effective visualizations. Each visualization is designed to directly address specific business questions and support data-driven decision-making:

- **Customer Preferences & Cuisine Ratings**: Identify which cuisines are most favored by customers and whether preferences differ across regions.

- **Price Perception & City Comparison**: Understand how pricing influences customer ratings and how price ranges vary across cities.

- **Cuisine Diversity & Ratings: Requirement**: Explore whether restaurants offering multiple cuisine styles perform better in terms of ratings.

- **Regional Insights & Market Opportunities**: Identify underrepresented or highly-rated niche cuisines to inform market strategy.

## Hypothesis and Validation

1. **Price Perception**

   - Hypothesis: Restaurants with higher prices are more likely to achieve better customer ratings.

   - Variables: Price Range (Low, Medium, High), Rating (Excellent, Average, Poor)

   - Validation Approach: Examine the correlation between rice range and rating using pie charts.

2. **Price Range vs. City**

   - Hypothesis: The the distribution of restaurant price ranges varies across different European cities. Wealthier European cities, such as Geneva and Zurich, have a higher proportion of expensive restaurants compared to cities like Budapest and Krakow.

   - Variables: Price Range, City

   - Validation Approach: Investigates the correlation between price range and city by using stacked bar chart and bar charts.

3. **Cuisine Counts vs. Rating**

   - Hypothesis: Restaurants offering a greater number of cuisines tend to receive higher customer ratings and potentially more reviews due to menu diversity.

   - Variables: Cuisines Counts, Rating

   - Validation Approach: Examine the correlation between cuisine counts and ratings using boxplot, line chart, bar charts and applying statistical testing.

4. **Cuisine-Based Preferences**

   - Hypothesis: Certain cuisines consistently receive higher customer ratings than others due to cultural preferences, dining experiences, and the inherent qualities of the cuisine.

   - Variables: Cuisine List, Rating, City

   - Validation Approach: Compare average ratings across different cuisines using bar charts in various cities and statistical testing.

5. **Cuisine vs. Price Range**

   - Hypothesis: Certain cuisines are associated with specific price ranges, reflecting differences in ingredients, preparation complexity, and dining experience. For example, French and Seafood cuisines are more likely to appear in higher price ranges, while Fast Food or casual cuisines dominate lower price categories.

   - Variables: Cuisine List, Price Range

   - Validation Approach: Analyze the relationship between cuisine type and price range using bar charts visualizations.

## Project Plan

| Phase                                  | Description                                                                                                                                                                                                                                                                 |
| -------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **1. Research Questions & Hypotheses** | Define the main analytical objectives and relationships to explore, including:<br>• Price perception and city-level variations<br>• City vs. price range<br>• Cuisine diversity and its effect on ratings<br>• Cuisine preferences<br>• Cuisine type vs. price relationship |
| **2. Data Collection**                 | Gather the dataset from [Kaggle](https://www.kaggle.com/datasets/damienbeneschi/krakow-ta-restaurans-data-raw/data)                                                                                                                                                         |
| **3. Data Cleaning & Preprocessing**   | • Handle missing values<br>• Standardize cuisine names<br>• Change/convert data types<br>• Remove duplicates<br>• Add new derived columns<br>• Drop unused columns<br>• Save the cleaned dataset as a new CSV file                                                          |
| **4. Exploratory Data Analysis (EDA)** | • Visualize key variable distributions<br>• Identify trends, patterns, and outliers<br>• Perform hypothesis testing (e.g., ANOVA, Tukey’s HSD) to validate findings                                                                                                         |
| **5. Dashboard Development**           | • Design a wireframe for an interactive dashboard<br>• Develop the dashboard in **Tableau**<br>• Display key metrics and visualizations aligned with research hypotheses                                                                                                    |
| **6. Key Insights & Conclusion**       | • Summarize main findings and observed patterns<br>• Highlight cultural and regional dining preferences<br>• Provide recommendations for improving restaurant strategies and market insights                                                                                |

## The rationale to map the business requirements to the data visualizations

## Analysis Techniques Used

## Ethical Considerations

- The dataset came from Kaggle and do not have any legal or societal issues. There was no personal data within the dataset which could expose or identify anything personal to a particular individual.

## Dashboard Design

## Wireframe

- The wireframe layout for EuroDine Insights Project was created using Figma to plan the structure and organization of key visual elements. It outlines where charts, maps, and summary cards will be placed, helping to ensure a clear and logical flow of information. This stage focuses on layout and functionality rather than design details, allowing for easy adjustments before building the actual dashboard.

![Wireframe](Images\wireframe.png)

## Tableau Dashboard

## Kanban Board

- You can find screenshots of our Kanban board [here](KANBAN.md)
- You can view the project board [here](https://github.com/users/RanaAlaaTahon/projects/3/views/1)

## Unfixed Bugs

## Development Roadmap

## Main Data Analysis Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn
- Plotly
- Tableau
- scipy

## Credits

- Kaggle Dataset: [TripAdvisor Restaurants Info for 31 Euro-Cities Dataset](https://www.kaggle.com/datasets/damienbeneschi/krakow-ta-restaurans-data-raw/data)
- Generative AI tools: ChatGPT, GitHub Copilot
- YouTube
- https://github.com/stephenbeese/Online-Retail-Analysis

## Acknowledgements
