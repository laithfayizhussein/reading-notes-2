# Pandas

- Pandas is a game-changer for data science and analytics, particularly if you came to Python because you were searching for something more powerful than Excel and VBA. Pandas use fast, flexible, and expressive data structures designed to make working with relational or labeled data both easy and intuitive.

- Customarily, we import as follows:

- In [1]: import numpy as np

- In [2]: import pandas as pd


# class pandas

- class pandas.DataFrame(data=None, index=None, columns=None, dtype=None, copy=False)

- Two-dimensional, size-mutable, potentially heterogeneous tabular data. Data structure also contains labeled axes (rows and columns). Arithmetic operations align on both row and column labels. Can be thought of as a dict-like container for Series objects. The primary pandas data structure.
## Parameters

- datandarray (structured or homogeneous), Iterable, dict, or DataFrame Dict can contain Series, arrays, constants, dataclass or list-like objects. If data is a dict, column order follows insertion-order.

- Changed in version 0.25.0: If data is a list of dicts, column order follows insertion-order.


- DataFrame.to_numpy() gives a NumPy representation of the underlying data. Note that this can be an expensive operation when your DataFrame has columns with different data types, which comes down to a fundamental difference between pandas and NumPy: NumPy arrays have one dtype for the entire array, while pandas DataFrames have one dtype per column. When you call DataFrame.to_numpy(), pandas will find the NumPy dtype that can hold all of the dtypes in the DataFrame. This may end up being object, which requires casting every value to a Python object.
- DataFrame.to_numpy() does not include the index or column labels in the output.

- describe() shows a quick statistic summary of your data.
- When selecting subsets of data, square brackets [] are used. Inside these brackets, you can use a single column/row label, a list of column/row labels, a slice of labels, a conditional expression or a colon.

    - Select specific rows and/or columns using loc when using the row and column names
    - Select specific rows and/or columns using iloc when using the positions in the table
    - You can assign new values to a selection based on loc/iloc.

- Getting data in to pandas from many different file formats or data sources is supported by read_* functions.
- Exporting data out of pandas is provided by different to_*methods.

