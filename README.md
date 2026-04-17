##Aim: Categorial Data Analysis using Python
##Theory:
Categorical Data Analysis involves the study of variables that represent discrete groups or labels rather than numerical measurements.
Categorical data analysis is a branch of statistics used to analyze data that can be divided into distinct groups. In Python, the pandas library is the primary tool for this.
These variables are typically classified into two types: Nominal and Ordinal.

##pd.read_csv(): Loads data from a CSV file into a structured DataFrame object.

##pd.DataFrame(): Creates a new DataFrame manually from a dictionary or list of data.

##value_counts(): Counts the unique occurrences of each value in a column.

##value_counts(normalize=True): Calculates the relative proportion (percentage as a decimal) of each unique value.

##unique(): Returns an array of all distinct categories present in a column.

##nunique(): Returns the total number of unique categories in a column.

##pd.crosstab(): Creates a frequency table (contingency table) to show the relationship between two categorical variables.

##pd.crosstab(..., normalize='index'): Normalizes the cross-tabulation by row to show percentages within each group.

##groupby(): Splits the data into groups based on a specific criteria for further calculation or analysis.

##df[df['col'] == 'val'] (Filtering): Extracts specific rows from the DataFrame that meet a defined condition.

##sort_values(): Reorganizes the rows of the DataFrame based on the alphabetical or logical order of a specific column.

##Conclusion:
The experiment successfully demonstrated how to process and interpret categorical datasets using the Pandas library.
