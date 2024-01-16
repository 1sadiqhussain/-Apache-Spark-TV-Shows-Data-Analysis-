# Apache-Spark-TV-Shows-Data-Analysis-
# Apache Spark Data Analysis 🚀

This Python script demonstrates data analysis using Apache Spark in a Google Colab environment. It covers the process of loading, exploring, and manipulating data, followed by insightful visualizations. Let's break down the code and how to use it.

## Setup Process 🛠️

1. **Install Java and Spark:**
   - Installs OpenJDK 8 and Spark 3.3.0 with Hadoop 3.
   
2. **Mount Google Drive:**
   - Mounts Google Drive to access Spark installation files.

3. **Environment Variables:**
   - Sets up Java and Spark environment variables.

4. **Initialize SparkSession:**
   - Initiates a SparkSession for handling computations.

5. **Load Libraries:**
   - Installs and initializes findspark to help Python locate PySpark module files.

## Data Loading and Exploration 📊

6. **Load Dataset:**
   - Reads the 'all_weeks_countries.csv' file into a Spark DataFrame.

7. **Display Table and Schema:**
   - Shows the loaded DataFrame and prints its schema.

8. **Separate Data:**
   - Creates two DataFrames, 'Films' and 'TV,' based on the 'category' column.

9. **Data Manipulation:**
   - Drops the 'season_title' column from the 'Films' DataFrame.
   - Replaces null values in 'season_title' in the 'TV' DataFrame with the corresponding 'show_title'.

10. **Group and Aggregate Data (Films):**
   - Groups data by 'country_name' and 'show_title,' finding the highest weekly rank and total weeks spent in the top 10 for each film.

11. **Find Most Popular Films by Country:**
   - Finds the film that spent the most time in each country's top 10 list.

12. **Convert to Pandas and Plot Pie Chart:**
   - Converts the DataFrame to a Pandas DataFrame and displays it as a pie chart.

13. **Group and Aggregate Data (TV):**
   - Groups data by 'country_name' and 'show_title,' counting the number of weeks each show appears in each country's top 10 lists and the highest weekly ranking.

14. **Find Most Popular TV Shows by Country:**
   - Finds the show that spent the most time in each country's top 10 list.

## Visualization and Insights 📈

15. **Pie Chart of Popular TV Shows:**
   - Displays a pie chart showing the distribution of popular TV shows across different countries.

## How to Use 🚀

- Execute the code cells sequentially in a Google Colab environment.
- Ensure the 'all_weeks_countries.csv' file is available in the specified file path.
- Explore the results and visualizations to gain insights into the popularity of films and TV shows across countries.

## Dependencies 📦

- PySpark
- Matplotlib
- Pandas

Feel free to customize and extend the analysis as needed. Happy coding! 🎉
