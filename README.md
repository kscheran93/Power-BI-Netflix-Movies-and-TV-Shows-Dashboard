
# Netflix Movies and TV Shows Dashboard

## Snapshot of Dashboard (Power BI Service)

![Dashboard_Snapshot](https://github.com/kscheran93/Power-BI-Netflix-Movies-and-TV-Shows-Dashboard/blob/main/netfilix%20.png)

### Dashboard Link: [https://app.powerbi.com/view?r=eyJrIjoiN2E5OGQ5NjEtODQ1ZS00YjJlLTljMzYtYzJkMjgyNmRhN2QyIiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9]

## Problem Statement

This dashboard provides insights into the Netflix movie and TV show catalog. It helps to analyze various aspects such as content type distribution, ratings, genres, release trends, and geographical distribution. By leveraging these insights, stakeholders can better understand the content library, viewer preferences, and potential gaps in the catalog. Additionally, the dashboard highlights trends in content releases over the years and identifies top countries contributing to Netflix's catalog.

### Steps Followed

- **Step 1:** Loaded the dataset into Power BI Desktop from a CSV file containing Netflix movies and TV shows data.

- **Step 2:** Cleaned and prepared the data using Power Query Editor, ensuring data integrity by checking for empty and erroneous values.

- **Step 3:** In the Report View, I selected a theme to make the dashboard visually appealing.

- **Step 4:** Created visualizations:
  - **Donut Chart:** Displays the distribution of content types (Movies vs. TV Shows). 
    - **Values:** Sum of `show_id`
    - **Legend:** `type`
  - **Horizontal Bar Chart 1:** Shows the distribution of content ratings.
    - **Y-Axis:** `rating`
    - **X-Axis:** Sum of `show_id`
  - **Horizontal Bar Chart 2:** Displays content distribution across different categories (genres).
    - **Y-Axis:** `listed_in`
    - **X-Axis:** Sum of `show_id`
  - **Area Chart:** Illustrates the trend in content releases over the years.
    - **X-Axis:** `release_year`
    - **Y-Axis:** Sum of `show_id`
  - **Treemap:** Highlights the geographical distribution of content across different countries.
    - **Category:** `country`
    - **Values:** Sum of `show_id`

- **Step 5:** Added visual filters:
  - **Top N Filter:** Selected the top 10 countries contributing the most content to the Netflix catalog.

- **Step 6:** Created six cards to display key metrics:
  - **Total Titles:** Represents the total number of titles in the dataset.
    - **Field:** `titles`
  - **Total Ratings:** Shows the total number of ratings available.
    - **Field:** `ratings`
  - **Total Genres:** Displays the total number of genres listed.
    - **Field:** `listed_in`
  - **Start Year:** Displays the earliest release year of content in the dataset.
    - **Field:** Minimum of `release_year`
  - **End Year:** Shows the most recent release year of content in the dataset.
    - **Field:** Maximum of `release_year`
  - **Locations:** Displays the count of unique countries where the content is produced.
    - **Field:** `count_of_country`

- **Step 7:** Published the report to Power BI Service for broader accessibility.

# Insights

The dashboard provides several key insights into Netflix's content catalog:

### [1] Content Type Distribution
   - The donut chart shows the split between Movies and TV Shows.
   - This helps understand the proportion of different content types available on Netflix.

### [2] Content Ratings
   - The horizontal bar chart reveals the distribution of content across different ratings.
   - This can help identify the most common ratings and guide decisions about content acquisition.

### [3] Content Categories
   - The second horizontal bar chart shows the distribution of content across various genres.
   - This gives insight into the diversity of content available.

### [4] Release Year Trend
   - The area chart illustrates how content production has evolved over the years, showing trends in new content releases.
   - This can highlight periods of high activity and potential shifts in content strategy.

### [5] Geographical Distribution
   - The treemap displays the countries that contribute the most content to Netflix.
   - Understanding the geographical distribution of content can help identify regional strengths and gaps.

### [6] Key Metrics
   - **Total Titles:** [8802]
   - **Total Ratings:** [18]
   - **Total Genres:** [515]
   - **Start Year:** [1925]
   - **End Year:** [2021]
   - **Locations:** [8807]

