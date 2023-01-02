# Pandas

## Pandas in 10

- Pandas is a game-changer for data science and analytics, particularly if you came to Python because you were searching for something more powerful than Excel and VBA. Pandas uses fast, flexible, and expressive data structures designed to make working with relational or labeled data both easy and intuitive.
- Creat a `Series` by passing a list of values, letting pandas create a default integer index.
- Creat a `DataFrame` by passing a NumPy array, with a datetime index using `date_range()` and labeled columns.
- Creating a `DataFrame` by passing a dictionary of objects that can be converted into a series-like structure.
- If you’re using IPython, tab completion for column names (as well as public attributes) is automatically enabled.
- Use `DataFrame.head()` and `DataFrame.tail()` to view the top and bottom rows of the frame respectively.
- Display with `DataFrame.index` or `DataFrame.columns`.
- `DataFrame.to_numpy()` gives a NumPy representation of the underlying data. Note that this can be an expensive operation when your `DataFrame` has columns with different data types, which comes down to a fundamental difference between pandas and Numpy
- NumPy: NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column. When you call `DataFrame.to_numpy()`, pandas will find the NumPy dtype that can hold all the dtypes in the DataFrame. This may end up being `object`, which requires casting every value to a Python object.
- For `df`, `DataFrame` of all floating-point values, and `DataFrame.to_numpy()` is fast and doesn’t require copying data.
- `describe()` shows a quick statistic summary of your data.
- `DataFrame.sort_index()` sorts by an axis.
- `DataFrame.sort_values()` sorts by values.
- Selecting a single column, which yields a `Series`, equivalent to `df.A`.
- electing via `[] (__getitem__)`, which slices the rows.
- Using the `isin()` method for filtering.
- pandas primarily uses the value `np.nan` to represent missing data. It is by default not included in computations.
- `DataFrame.dropna()` drops any rows that have missing data.
- `DataFrame.fillna()` fills missing data.
- `isna()` gets the boolean mask where values are `nan`.
- `DataFrame.apply()` applies a user defined function to the data.
- Series is equipped with a set of string processing methods in the `str` attribute that make it easy to operate on each element of the array, as in the code snippet below. Note that pattern-matching in `str` generally uses regular expressions by default (and in some cases always uses them).
- pandas provides various facilities for easily combining together Series and DataFrame objects with various kinds of set logic for the indexes and relational algebra functionality in the case of join / merge-type operations.
- Concatenating pandas objects together along an axis with `concat()`.
- `merge()` enables SQL style join types along specific columns.
- Splitting the data into groups based on some criteria
- Applying a function to each group independently
- Combining the results into a data structure
- The `stack()` method “compresses” a level in the DataFrame’s columns
- With a “stacked” DataFrame or Series (having a `MultiIndex` as the index), the inverse operation of `stack()` is `unstack()`, which by default unstacks the last level.
- 
### Sources

- <https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html>
- <https://realpython.com/learning-paths/pandas-data-science/>

[Back To Home](../README.md)