# Data Analysis
***
## freeCodeCamp [Course](https://www.freecodecamp.org/learn/data-analysis-with-python/) Notes

### [Introduction to Data Analysis](https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-course/introduction-to-data-analysis)

###### What is data analysis?
A process of inspecting, cleansing, transforming and modelling data with the goal of discovering useful information, informing conclusions and supporting decision making.

###### Data Analysis tools
We can categorize the tools into two main categories. Managed-closed and Open-source

For example:
|Managed-closed|Open source|
|-|-|
|QlikQ|Python|
|Tableau|R|
|Zoho Analytics|Julia

Why am I going to use python to learn data analysis?
 - Simple and easy to learn
 - Free
 - Huge support community and libraries

###### Data Analysis Process
![alt](img/sc-fcc-datapipeline.png)

###### Python libraries
- **pandas:** The cornerstone of DA
- **matplotlib:** A library for *visulisations*
- **numpy:** *numeric* library that will perform calculations
- **seaborn:** A *statistical visualisation* built on top of matplotlib
- **statsmodels:** *Statistical* functions
- **scipy:** Advanced *scientific computing* including optimisation and linear algebra
- **scikit-learn:** Most popular *machine learning* library for python (not deep learning)

###### How is DA using Python different from traditional methods?
Using a traditional tool like excel, we can visualise the data within a spreadsheet. We can perform DA on top of the original data. However when using Python, you are not constantly looking at the data which allows for greater quantities, speed and efficiency of processing for data. 

### [Data Analysis Example Part 1](https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-course/data-analysis-example-a)

The dataset used is a CSV file composed of sales data. It is loaded from the CSV to a Pandas Dataframe.

The shape of the dataframe tells us the total number of rows and columns present in the dataset.

You can call info method on the dataframe to get an idea on the datatypes of each of the columns.

We can use the .describe() to get quick statistics on the numeric values of the data. E.g. mean, median, max and min. 

### [Data Analysis Example Part 2](https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-course/data-analysis-example-b)

This video first looks to show the speed of processing from Excel vs Python. 

The then goes on to do some some validation by creating a new calculated column and comparing it with an existing column from the dataset. 

The course then demonstrates some quick filtering of the data.

### [How to use Jupyter Notebooks Intro](https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-course/how-to-use-jupyter-notebooks-intro)

**Why do we use a Jupyter Notebook?**
- It is a highly interactive place to code.
- We can output data at any point of the code.
- We can create a command and immediately get a response. 
- A cell can use code or markdown. Making it highly workable
- Keyboard shortcuts
- Interactive data visualization
- Working with other filetypes like Excel

### [Introduction to Numpy](https://www.freecodecamp.org/learn/data-analysis-with-python/data-analysis-with-python-course/numpy-introduction-a)

Processing numbers in python is quite slow. Numpy solves that. It sits on top of python to perform high performance numeric computations.

Usually we do not see numpy being explicitly deployed. It actually makes up fundamental parts of other python libraries like Pandas.

Numpy is effecient in two ways:
###### Number storage
- Small numbers only need a certain number of bits to be stored. However because python stores numbers as an integer object, it often takes a large fixed size which is 100x more than the number of bits needed to store that number. 
- Imagine dealing with millions of rows of data like this, it is very inefficient.
- Numpy uses the correct number of bits to store and process number.

###### Array processing
- Stores numbers in arrays which are stored next to each other in memory. Allows for CPU to run low-level efficient quick calculations.
- Python lists can store numbers all over the memory. And they are stored in as integer objects so can not be directly processed by the CPU. 