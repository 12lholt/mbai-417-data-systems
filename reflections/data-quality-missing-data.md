# Data Quality / Missing Data Reflection

Team members: Nick Wright, Patrick Galvin, Waris-sara Buajeeb 

TL;DR - Most data needs to be enhanced before it's completely useful for models. You will need to choose the most appropriate methods available to fill in missing data in your dataset, and there are some built-in libraries in Python/Pandas to help with that.

## Lecture Recap

### Data quality / Missing data issues
- Based on statistical survey from O’Reilly 2019 AI Adoption survey, data quality or missing data issue are considered as top issue for AI project, especially during AI implementation. 

- Missing data can be viewed based on the level of Missing At Random (MAR), which ranging from Missing Not At Random (MNAR) to Missing Completely At Random (MCAR).

- Most businesses require high-quality data to deliver value in business decisions.  

### Data Quality Definition
- Data quality can be measured and categorized into 5 aspects (Accuracy, Completeness, Timely, Consistency, Unique) 

- It’s essential to manage the data based on the above aspects to ensure that data can be utilized later in data analytics, machine learning or AI model 

- Completeness of data refers to the evaluation of whether all data is presented in the system, is there any missing field in systems. 

### Examples in business worlds / industries
- Power outages (such as the Texas temperature sensors we observed in class)
- Ommitted answers from survey data
- Consistent unites of measurement; it's always a good idea to transform your data into standard units (such as time in UTC) before joining data sets. 
- At times, data can be stored in a way that needs to be manipulated in order to be joined with adjacent systems. An example of this is when we took temperature data from different sensors in the homework, and had to "pivot" the data so that we could have it organized in a way that could be linked with the power generation data (joined by date).


## Key implications and takeaways

### How to handle missing data with Python
We can use Python library – Pandas to conduct data analysis and manipulation. DataFrames in pandas is able to handle and analyze huge amounts of data. 

Types with accompanying definitions: We have a choice as to how to deal with missing data with dataframes as follows: 

- Fill NA with Mean, Median or Mode of the data: This option allows us to introduce values that don't impact the overall dataset 

- Fill NA with a constant value: To fill specific value instead of NA-marked value. This value might frequently be Zero, or based on your business intuition, some default number that makes intuitive sense.

- Backward Fill: To fill missing values with the first non-missing value that occurs after it. 

- Forward Fill: To fill missing values with the first non-missing value that occurs before it 

- Interpolation: To use mathematical interpolation to determine which value should have been put in the missing data. This could be as simple as taking the average of the last known value and the next known value for a particular feature.

### Preventing Poor Data
If you have a chance to impact how the data is collected upstream, you can create a lot of value for the future data analysis and machine learning pipeline.

- To avoid missing data in surveys, a common technique is to include a "Don't Know" or "Refused to answer" option for respondents

- To improve your data quality, it's often useful to have your data structured in third normal form (like we learned in 417). This prevents features from being mispelled or referenced multiple times, and allows for better backfilling techniques by conditional probabilities.


## Additional Resources

### Handling Missing Data with Python/Pandas
- Python: How to Handle Missing Data in Pandas DataFrame (stackabuse.com)
https://stackabuse.com/python-how-to-handle-missing-dataframe-values-in-pandas/

### Classifying pattern of missing data

- Recognizing different patterns of missing data (towardsdatascience.com) https://towardsdatascience.com/the-problem-of-missing-data-9e16e37ef9fc


### Impact of Poor Data Quality

 - Describes a framework for dealing with poor data quality when implementing Machine Learning processes (hbr.org) https://hbr.org/2018/04/if-your-data-is-bad-your-machine-learning-tools-are-useless