# Data Analysis

## What is Jupyter Lab

- <https://youtu.be/A5YyoCKxEOU>
- JupyterLab enables you to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner.
- You can arrange multiple documents and activities side by side in the work area using tabs and splitters. Documents and activities integrate with each other, enabling new workflows for interactive computing.
- JupyterLab also offers a unified model for viewing and handling data formats. JupyterLab understands many file formats (images, CSV, JSON, Markdown, PDF, Vega, Vega-Lite, etc.) and can also display rich kernel output in these formats.
- Code Consoles provide transient scratchpads for running code interactively, with full support for rich output. A code console can be linked to a notebook kernel as a computation log from the notebook, for example.
- Kernel-backed documents enable code in any text file (Markdown, Python, R, LaTeX, etc.) to be run interactively in any Jupyter kernel.
- Notebook cell outputs can be mirrored into their own tab, side by side with the notebook, enabling simple dashboards with interactive controls backed by a kernel.
- Multiple views of documents with different editors or viewers enable live editing of documents reflected in other viewers. For example, it is easy to have live preview of Markdown, Delimiter-separated Values, or Vega/Vega-Lite documents.

## Numpy Tutorial
- NumPy is a commonly used Python data analysis package. By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem, like scikit-learn, that use NumPy under the hood.
- NumPy was originally developed in the mid 2000s, and arose from an even older package called Numeric. This longevity means that almost every data analysis or machine learning package for Python leverages NumPy in some way.
- ssv (semicolon separated values) format — each record is separated by a semicolon (;), and rows are separated by a new line.
- A 2-dimensional array is also known as a matrix, and is something you should be familiar with. In fact, it’s just a different way of thinking about a list of lists. A matrix has rows and columns. By specifying a row number and a column number, we’re able to extract an element from a matrix.
- In a NumPy array, the number of dimensions is called the rank, and each dimension is called an axis. So the rows are the first axis, and the columns are the second axis.
- We can create a NumPy array using the numpy.array function. If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns.
- One of the limitations of NumPy is that all the elements in an array have to be of the same type, so if we include the header row, all the elements in the array will be read in as strings.
- We can use array indexing to select individual elements, groups of elements, or entire rows and columns. One important thing to keep in mind is that just like Python lists, NumPy is zero-indexed, meaning that the index of the first row is 0, and the index of the first column is 0.
- A colon indicates that we want to select all the elements from the starting index up to but not including the ending index. This is also known as a slice
- We can select an entire column by specifying that we want all the elements, from the first to the last. We specify this by just using the colon (:), with no starting or ending indices.
### Sources

- <https://jupyterlab.readthedocs.io/en/stable/getting_started/overview.html>
- <https://www.dataquest.io/blog/numpy-tutorial-python/>

[Back To Home](../README.md)