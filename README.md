Theory:
Categorical data analysis is the study of data that represents categories or groups. In Python, it is performed using libraries like pandas and numpy to calculate frequencies, visualize data, and analyze relationships.
import pandas- This line imports the pandas library.Pandas is used for data handling and analysis.
pd.read_csv("/content/Expt11.csv")-It reads the CSV file from the given path and stores it as a dataFrame in Python.
df.shape- It returns the dimensions of the dataframe in the form of (rows,columns).
df.size- It returns the total number of elements (values) in the dataFrame.(size=rows*columns).
df.info() is a function used to get a summary of a dataframe.
It gives number of entries (rows), column names, non-null values, data types and memory usage.
df.head-It is used to display the first few rows of a dataframe.By default, it shows first 5 rows.
df.tail-It is used to display the last few rows of a dataframe.By default, it shows last 5 rows.
df.sample(5) is used to select random rows from a dataframe.It returns 5 random rows from the dataset.
df.isnull().sum()-It is used to check missing (null) values in each column of a datarfame.
df.duplicated().sum()-It is used to find the number of duplicate rows in a dataframe.
df.nunique() is used to count the number of unique (distinct) values in each column of a dataframe.
df['Grade'].value_counts()-It returns the frequency (count) of each unique category in the 'Grade' column.
df['Gender'].value_counts()-It returns the frequency (count) of each unique category in the 'Gender' column.Similarly we can calculate for other columns like department.
df['Grade'].value_counts(normalize=True)*100-It returns the percentage distribution of each category in the 'Grade' column.
(pd.crosstab(df['Gender'],df['Grade'])-It creates a contingency table showing the frequency of each combination of Gender and Grade.Similarly, 'Department' vs 'Gender' and 'Department' vs 'Grade' can be calculated.
(pd.crosstab(df['Department'],df['Grade'],normalize='index')*100)-It shows the row-wise percentage distribution of Grade within each Department.
df.groupby('Department')['Grade'].value_counts()-It returns the count of each Grade within each Department (group-wise frequency).
pd.DataFrame(data)-It creates a DataFrame from the given data using the pandas library.
df['Category'].value_counts()-It returns the frequency (count) of each unique category in the 'Category' column.In similar way unique payment methods can be calculated.
df['Category'].value_counts(normalize=True)*100-It returns the percentage distribution of each category in the 'Category' column.
df['Category'].unique()-It returns all unique values (distinct categories) present in the 'Category' column.
df['Category'].nunique()-It returns the number of unique (distinct) categories in the 'Category' column.
pd.crosstab(df['Category'],df['Payment_Method'])-It creates a contingency table showing the frequency of each combination of Category and Payment Method.
df[df['Category']=='Electronics']-It filters the DataFrame and returns rows where the Category is 'Electronics'.
df.sort_values(by='Category')-It sorts the DataFrame in ascending order based on the 'Category' column.
df.groupby('Category')['Payment_Method'].value_counts()-It returns the count of each Payment Method within each Category (group-wise frequency).
Sorting: Sorted categorical data for better analysis.
Unique Values: Identifies unique categories using unique() and nunique.
Functions / Commands Used:
pd.read_csv() → Load dataset.
head() → Display first few rows.
value_counts(normalize=True) → Percentage distribution.
pd.crosstab() → Cross-tabulation between variables.
groupby() → Group data based on categories.
size() → Count elements in each group.
count() → Count non-null values.
unique() → Get unique values.
nunique() → Count unique values.
sort_values() → Sort data.
isin() → Filter specific category values.
loc[] → Filter rows based on conditions.
Conclusion:
Categorical data analysis using python helps in understanding and interpreting qualitative data efficiently.
With libraries like pandas and matplotlib, we can easily perform frequency analysis, comparisons, visualization, and statistical testing.
