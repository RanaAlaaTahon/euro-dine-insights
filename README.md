# **EuroDine Insights**

**EuroDine Insights**

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

  - Name: name of the restaurant

  - City: city location of the restaurant

  - Cuisine Style: cuisine style(s) of the restaurant, in a Python list object.

  - Ranking: rank of the restaurant among the total number of restaurants in the city as a float object.

  - Rating: rate of the restaurant on a scale from 1 to 5, as a float object.

  - Price Range: price range of the restaurant among 3 categories , as a categorical type.

  - Number of Reviews: number of reviews that customers have let to the restaurant, as a float object.

  - Reviews: 2 reviews that are displayed on the restaurants scrolling page of the city, as a list of list object where the first list contains the 2 reviews, and the second le dates when these reviews were written.

  - URL_TA: part of the URL of the detailed restaurant page that comes after 'www.tripadvisor.com' as a string object.

  - ID_TA: identification of the restaurant in the TA database constructed a one letter and a number.

  ## Business Requirements

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

     - Validation Approach: Examine the correlation between cuisine counts and ratings using boxplot, line chart and bar charts.

  4. **Cuisine-Based Preferences**

     - Hypothesis: Certain cuisines consistently receive higher customer ratings than others due to cultural preferences, dining experiences, and the inherent qualities of the cuisine.

     - Variables: Cuisine List, Rating, City

     - Validation Approach: Compare average ratings across different cuisines using bar charts in various cities.

  5. **Cuisine vs. Price Range**

     - Hypothesis: Certain cuisines are associated with specific price ranges, reflecting differences in ingredients, preparation complexity, and dining experience. For example, French and Seafood cuisines are more likely to appear in higher price ranges, while Fast Food or casual cuisines dominate lower price categories.

     - Variables: Cuisine List, Price Range

     - Validation Approach: Analyze the relationship between cuisine type and price range using bar charts visualizations.

  ## Project Plan

- Define Research Questions & Hypotheses:

  - Identify the key relationships to explore: price perception, city vs price range, cuisine diversity and ratings, cuisine preferences, and cuisine vs price.

- Data Collection:

  - Gather the dataset from Kaggle

- Data Cleaning & Preprocessing:

  - Handle missing values
  - Standardized cuisine names
  - Change data types
  - Remove duplicates
  - Add new columns
  - Drop unused columns

- Save the cleaned data to a new CSV file

- Exploratory Data Analysis (EDA):

  - Visualize distributions of key variables, identify trends, outliers, and patterns.
  - Hypothesis Testing

- Dashboard Creation

  - Design and develop an interactive dashboard by first creating a wireframe and then implementing it in Tableau.
  - The dashboard will showcase key metrics and visualizations that align with and support the hypotheses.

- Project Key Insights and conclusion

  ## The rationale to map the business requirements to the data visualizations

  ## Analysis Techniques Used

  ## Ethical Considerations

- The dataset came from Kaggle and do not have any legal or societal issues. There was no personal data within the dataset which could expose or identify anything personal to a particular individual.

## Dashboard Design

## Wireframe

![Wireframe]()

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
- Scikit learn

## Credits

- Kaggle Dataset: [TripAdvisor Restaurants Info for 31 Euro-Cities Dataset](https://www.kaggle.com/datasets/damienbeneschi/krakow-ta-restaurans-data-raw/data)
- Generative AI tools: ChatGPT, GitHub Copilot
- YouTube
- https://github.com/stephenbeese/Online-Retail-Analysis

## Acknowledgements
