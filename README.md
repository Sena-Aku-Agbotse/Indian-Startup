# **Indian-Startup Funding Analysis Project**


# **Project Objective**
In this project,my team and I investigate the evolving landscape of start-up funding in India from 2018 to 2021. Our goal is to identify key patterns, trends, and insights that define the investment ecosystem during this period. The dataset for this analysis was sourced from different platforms,that is,Microsoft SQL server, OneDrive and a GitHub repository


# **Project Structure**

 **Objective**

In this phase, we outline the business goals, develop hypotheses, and pose questions to support or refute these hypotheses. Additionally, we aim to gain general insights into the data.


**Business Task**
As the data experts,our task is to analyze  the Indian start-up data to provide valuable insights and guidance for my client seeking to enter the Indian start-up ecosystem. My goal is to highlight key metrics and considerations that will inform their decisions before entering this dynamic market.


**Hypothesis**
Null Hypothesis (H0) – The funds a company receives does not depend on the sector the company invests in.
 
Alternative Hypothesis (H1) – The funds a company receives depends on the sector a company invests in.


**Business Questions**
1. What are the top five(5) attractive sectors?
2. How does funding vary with the location of start-ups? 
3. What are the average funding amounts for different funding stages(e.g, Seed, Series A, Series B etc).
4. What is the total funding amounts per sector?
5.	How does funding vary within the various geographical locations for start-ups?




**Deliverables**
A hypothesis.
Questions to help gain insights into the data.
A summary of the analysis.
Visualizations to communicate findings.
Recommendations based on the analysis.

**Data Preparation and Quality Check**
In this phase, we retrieved data from multiple sources for analysis.

**Information on Data**
The data for the project was provided by Azubi Africa. The data contains four CSV files: data_2018.csv, data_2019.csv, data_2020 (from SQL Server), and data_2021 (also from SQL Server).

**Columns in the Data**
Company Name: The name of the company.
Founded: The year the company was founded.
Sector: The sector the company operates in.
Stage: The funding stage of the company.
Location: The location of the company’s headquarters.
Amount: The amount of funding the company received.
Description: Information about the company.
Investor: The investor who funded the company.
Founder: The founders of the company.

**Data Limitations**
The 2018 start-up data lacks two columns (Founders, Founded) that are present in the 2019, 2020, and 2021 datasets. Additionally, the source of the 2018 dataset is unknown, making this data unreliable for making real-life recommendations for entrepreneurs.

**Data Selection**
All four datasets (2018-2021) were retrieved from their respective sources for the purpose of this analysis.

**Tools for Analysis**
We utilize the following tools:

Python's:
Pandas: For data manipulation and cleaning.
NumPy: For numerical operations.
Matplotlib and Seaborn: For data visualization.
SQL: For querying and managing the 2020 and 2021 data stored in Microsoft SQL Server.
GitHub: To access the 2018 dataset and manage version control for any scripts or notebooks used in the analysis.
Jupyter Notebook: For interactive data analysis and sharing insights through well-documented notebooks.


# **Technical Content**

**Exploratory Data Analysis(EDA)**
Here,we summarized the main characteristics of all the datasets from 2018 to 2021. This was done to understand patterns,check assumptions,detect anomalies and test our hypothesis.

1. We imported our data from various sources(GitHub repository and CSV files)

2. We previewed the rows and columns and went ahead to check for information on the various datasets.

3. We checked for the datatypes of each column.

4. We further checked for missing and duplicated values.
 
 - Some key issues were observed after going through with this EDA,they are:

 - Different currencies in amounts.
 - Column inconsistencies and irrelevant columns.
 - Missing data.
 - Inconsistent values in categorical features.

 **Data Cleaning and Preparation**

 - Convert Indian Rupees to dollars,add the years each dataset was collected. We then merge the columns and rename the columns. Cleaning begins from here on.

 **Cleaning all columns**

 1. Amount column
 - Here, we remove all unwanted symbols
 - Change column from object to float 
 - Fill in null values.


 2. Founded column
 - Covert this column to numeric
 - Fill null values with interpolate method
 - Convert to datetime
 - Convert to period


 3. Founders column
 - Take out unwanted symbols
 - Check for Nan values


 4. Headquarter column
 - Check and  drop duplicates
 

 5. Sector column
 - Standardize the names of sectors
 - Check for information


 **Hypothesis testing**
 - We extract only the 'sector' and 'amount' columns from our dataset.
 - Remove any rows with missing values
 - Group data by sector and perform one-way ANOVA test to see if the amount of funding depends on the sector.
 - Set a threshold(0.5) to decide if the result is statistically significant.
 - Interpret and print out the result.
 

 **Answering analytical questions**
 - We explored our data and answered our questions based on that.



# **Recommendations/Conclusion**
1.Location Focus:
Investors should concentrate on top-funded cities such as Mumbai, Shanghai, San Francisco, Kalpakkan, and Beijing.

2.Sector Investments:
Look for opportunities in fintech and retail, the most attractive sectors for investors.

3.Trend Monitoring:
Keep an eye on trends in mature startups in the 'Others' category, indicating investor confidence in later-stage ventures.

4.Portfolio Diversification:
Diversify investments across locations and sectors to achieve a balanced risk-return profile.

# **Appreciation**
I highly recommend Azubi Africa for their comprehensive and effective programs and our able intstructors.






