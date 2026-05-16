# Understanding Why Customers Leave: A Telco Churn Analysis

The project aims to analyze customer churn in a telecommunications company and develop predictive models to identify at-risk customers. The ultimate goal is to provide actionable insights and recommendations to reduce churn and improve customer retention.

A data analytics project exploring customer churn patterns in a telecommunications dataset.  
Performed end-to-end analysis: data cleaning, exploratory data analysis (EDA), and interactive visualizations using Python (Pandas, Matplotlib, Seaborn, Plotly).  

Key insights:  
- Short-tenure customers churn more often.  
- Higher monthly charges correlate with higher churn.  
- Long-term customers tend to pay lower monthly charges.  

Tools: Python- Jupyter Notebook (Pandas, NumPy, Matplotlib, Seaborn, Plotly Express, Plotly Graph Objects)

My Learning Journey

When I started this project, I already knew basic Python syntax and a little bit of Pandas. But turning a messy CSV into clear business insights felt like a big step.

Step 1 – Understanding the data  
I loaded the Telecommunication Customer Churn dataset and immediately noticed mixed data types and missing values in the TotalCharges column. At first I was confused, but after reading documentation I realized I needed to convert it to numeric with errors='coerce'. That small parameter taught me how to handle real-world data imperfections.

Step 2 – Cleaning and preparation  
I standardized column names (lowercase + underscores), checked for duplicates (none), and dropped rows where TotalCharges became NaN. Nothing fancy – but essential.

Step 3 – Exploratory Data Analysis (EDA)  
This is where things got visual. I used Seaborn (imported as sb) for quick statistical plots, and Matplotlib for customizing. I created histograms of tenure, boxplots of monthly charges, and bar charts of churn vs non-churn.

Step 4 – Segmentation & advanced visuals  
I grouped customers by tenure (0–12, 13–36, 37+ months) and built a donut chart using Plotly Graph Objects – my first interactive chart! Then a clustered bar chart with annotations to show average monthly charges per group.  

I also analyzed churn by demographic factors (gender, senior citizen), payment methods, and contract types. The patterns were clear: month-to-month contracts and electronic check payments had the highest churn.

Step 5 – Connecting insights to business  
The biggest "aha" moment was seeing that shorter tenure + higher monthly charges almost always leads to churn. I also noticed long-term customers pay less on average – probably due to discounts or loyalty plans.

Challenges I solved myself:
- Plotly Express vs Graph Objects: I initially mixed them up. After trial and error, I learned that px is great for quick charts, while go gives more control.
- TotalCharges conversion: I accidentally dropped too many rows at first because I didn't check how many missing values there were. I recalculated and found only ~10 rows – safe to drop.

Technical Skills:
- Data cleaning with Pandas (dropna, to_numeric, duplicated, rename columns)
- Handling missing values & type conversion (errors='coerce')
- Static visualization: Matplotlib (plt) and Seaborn (sb)
- Interactive visualization: Plotly Express (px) and Plotly Graph Objects (go)
- Grouping & aggregation for segmentation (pd.cut, groupby)
- Histograms, boxplots, bar charts, line graphs, donut charts

Analytical Skills:
- Identifying churn drivers (tenure, monthly charges, contract type, payment method)
- Customer segmentation by tenure groups
- Comparing average monthly charges across segments
- Interpreting visual patterns to form business recommendations

Soft / Practical Skills:
- Debugging data type issues in real-world datasets
- Choosing between static vs interactive plots based on audience
- Writing clear, reproducible analysis code in Jupyter Notebook
- Translating technical findings into business-friendly language

Overall, this project taught me that data analysis is not about perfect code – it's about asking the right questions and cleaning enough to find honest answers.
