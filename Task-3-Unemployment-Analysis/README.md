This project performs an exploratory data analysis (EDA) of unemployment data in India. The Python script uses libraries like Pandas for data manipulation and Matplotlib and Seaborn for data visualization to uncover trends and patterns related to unemployment, labour participation, and employment rates.

1. Data Processing and Cleaning
The script starts by loading the Unemployment in India.csv dataset. It then cleans the data by standardizing column names, converting the date column to a proper datetime format, and ensuring consistency in state names. This preprocessing step is crucial for accurate analysis.

2. Key Insights and Visualizations
The script generates several plots to provide a comprehensive overview of the unemployment landscape:

National Unemployment Trend: A line plot illustrates the national average unemployment rate over time, showing its fluctuation.

State-wise Heatmap: A heatmap visualizes the unemployment rate for each state across different dates, helping to identify regional variations and trends.

Latest State-wise Unemployment: A barplot displays the unemployment rates for all states on the most recent date, allowing for a quick comparison of which states have the highest rates.

Urban vs. Rural Comparison: A boxplot compares unemployment rates in urban and rural areas, highlighting any significant differences between them.

Labour Participation Trend: A line plot also tracks the national average labour participation rate over time, which provides context on the size of the workforce.

Top 10 States: A dedicated barplot highlights the top 10 states with the highest unemployment rates, pinpointing areas that may require more attention.

All generated plots are saved as .png files in the Task-3-Unemployment-Analysis/results/ directory. This organized approach makes it easy to review the findings and share the results.
