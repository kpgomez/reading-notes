# Class 12

## Sources

- [Pandas in 10](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)
- [Pandas - Getting Started](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)
- [Corey Schafer - Panda Tutorials](https://www.youtube.com/playlist?list=PL-osiE80TeTsWmV9i9c58mdDCSskIFdDS)

## Notes
`import pandas as pd`
THere are two types of classes for handling data: Series and DataFrames. Series are one-dimensional. DataFrames are two-dimensional. Create Series by passing in a list of values of a single datatype and DataFrame by passing in a NumPy array, anything that can be represented as rows and columns with varying datatypes for each column. ***Each column in a DataFrame is a Series***

Syntax for creating Series
`variable_name = pd.Series(data, index=index)`
index is a list of axis labels
The series' default row labels look like indices

Syntax for creating DataFrames
`variable_name = pd.DataFrame(data, index=index)`
use DataFrame.head() to view top and DataFrame.tail() to view bottom of frame

Selecting columns in a DataFrames is similar to how dictionary keys are selected

use DataFrame.to_numpy() to view NumPy representation of the underlying data

List of DataFrame methods/attributes

![Alt text](<Screenshot 2023-10-24 at 4.40.04 PM.png>)



## Bookmark and Review
- [Master Pandas](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386)
- [Panda Cookbook](https://pandas.pydata.org/pandas-docs/stable/user_guide/cookbook.html#cookbook)

## Reading Questions
1. Explain the purpose and basic functionality of the Pandas library. What are some common operations that can be performed on data using Pandas, and how do they contribute to data analysis and manipulation? Panda is a powerful data analysis/manipulation library that can handle and transform extremely large datasets common in Big Data with ease. Panda together with NumPy are essential data science tools. 

2. What are the primary data structures in Pandas, and how do they differ in terms of use cases? The primary data structures are Series and DataFrames. Series can hold only one datatype. A DataFrame is made of Series and each Serie can hold a different datatype. 

3. Describe the process of loading a dataset into a Pandas DataFrame. What are some common file formats that can be used, and which Pandas functions are utilized to read these formats? Load data by reading it using this syntax `data = pd.read_csv('my_file.csv')`. Common file formats include text formats like csv, JSON, HTML, XML; binary formats like MS Excel, SAS and SQL formats like SQL and Google BigQuery. 



