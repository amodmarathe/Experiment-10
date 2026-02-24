Amod Marathe 25070123073
Exp 10

The pandas library is the primary open-source library for data manipulation and analysis in Python, widely used across academic and commercial domains including finance, science, and machine learning.

pd.Series- This creates a one-dimensional labeled array called a Series. In your code, s = pd.Series([10,20,30,40,55]) creates a Series containing these numbers with a default integer index.
p.DataFrame(data): This creates a two-dimensional labeled data structure with columns of potentially different types, known as a DataFrame. It's similar to a spreadsheet or SQL table. Your code uses a dictionary data to define the column names and their corresponding values.
df.shape: This attribute of a DataFrame returns a tuple representing its dimensions (number of rows, number of columns).

df.ndim: This attribute returns the number of dimensions of the DataFrame (which is always 2 for a DataFrame).
df.size: This attribute returns the total number of elements (cells) in the DataFrame, which is the product of rows and columns.
df.columns: This attribute returns the column labels (names) of the DataFrame as an Index object.

df.dtypes: This attribute returns a Series with the data type of each column in the DataFrame.
df.loc[row_index, "Column Name"]: This is a label-based indexer used to access a group of rows and columns by their labels. For example, df.loc[0,"Name"] retrieves the value in the 'Name' column for the row with label 0.
df.iloc[row_position, column_position]: This is an integer-location based indexer used to access a group of rows and columns by their integer positions. For example, df.iloc[2,1] retrieves the value at the third row (index 2) and second column (index 1).

df.iloc = value: This is used to update the value of a specific cell in the DataFrame using its integer-based row and column positions. For example, df.iloc[0,1]=88 changes the value in the first row, second column to 88.
df.drop("column_name", axis=1): This method is used to remove a specified column (or row). axis=1 indicates that you are dropping a column. This method returns a new DataFrame with the specified column removed, leaving the original DataFrame unchanged unless reassigned.
df["Column Name"].mean(): This calculates the arithmetic mean (average) of the values in the specified column.

df["Column Name"].min(): This finds the minimum value in the specified column.
df["Column Name"].max(): This finds the maximum value in the specified column.
df[df["Column Name"] > value]: This is a common way to filter a DataFrame based on a condition. df["Column Name"] > value creates a boolean Series (True/False for each row), and when used to index the DataFrame, it returns only the rows where the condition is True.
