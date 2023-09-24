# Energy Consumption Analysis 🌍🔌

This repository contains Python code for analyzing energy consumption data from a PostgreSQL database. The data includes information about energy consumption, renewable energy share, and electricity generation for various countries. The code uses the SQLAlchemy library to connect to the database, execute SQL queries, and perform data analysis and visualization using pandas and matplotlib.

## Getting Started 🚀

Before running the code, ensure you have the following prerequisites:

- The data that can be found here https://www.kaggle.com/datasets/pralabhpoudel/world-energy-consumption
- A PostgreSQL database (I suggest elephantSQL free instances!)
- Python installed on your system
- Required Python libraries: SQLAlchemy, pandas, and matplotlib

You can install the required libraries using pip:

```bash
pip install SQLAlchemy pandas matplotlib
```

## Code Overview 📃

### Data Loading 📊

The code starts by creating a PostgreSQL database engine using a specified URL. It then defines a function `load_csv_to_postgres` to load CSV data into PostgreSQL. Note that this function is currently commented out, so you need to uncomment and modify it to load your CSV data into the database.

### SQL Query Execution ⚙️

The code defines a function `execute_query` to execute SQL queries. It establishes a connection to the PostgreSQL database, executes the query, fetches the results into a DataFrame, and closes the connection.

### Data Analysis and Visualization 📈

The code includes several SQL queries to analyze and visualize energy consumption data. Here are the key analyses performed:

1. **Top Countries by Renewables Share of Energy**: This analysis identifies the top countries with the highest renewables share of energy and visualizes the data using a bar chart.

2. **Top Countries by Renewables Share of Electricity**: Similar to the first analysis, this one focuses on renewables' share of electricity consumption.

3. **Canada's Renewable Energy Trends**: This section explores Canada's renewable energy trends, comparing its renewables share of energy and electricity consumption to the world average. Line plots are used to visualize these trends.

4. **Canada's Annual Growth in Renewables Electricity**: This analysis examines Canada's annual growth rate in renewables electricity generation using a line plot.

5. **Canada's Annual Growth in Low-Carbon Electricity**: Similar to the previous analysis, this one looks at the annual growth rate of low-carbon electricity generation in Canada.

6. **Renewables vs. Fossil Fuels in Canada**: This analysis uses a stacked area plot to visualize the percentage of electricity consumption in Canada from renewables and fossil fuels over the years.

### Saving Data 💾

The code saves the query results in dataframes, which are then saved in CSV files (in this case, with a `.txt` extension for a specific use case). However, you can easily modify the code to save data in various formats, such as Excel, or even back to the database. The possibilities are immense, and you can create visualizations using your favorite tools such as Power BI and Tableau.

## Conclusion 🌟

This code provides a comprehensive analysis of energy consumption data, focusing on renewables, low-carbon sources, and Canada's energy trends. You can adapt the code and queries to analyze data specific to your PostgreSQL database. Remember to configure the database URL and uncomment the data loading function if necessary.

This project is a work in progress, and as it continues to develop, the goal is to answer questions like: "How sustainable is Canada when it comes to the energy market?" Stay tuned for further developments and insights. 🍁🌿
