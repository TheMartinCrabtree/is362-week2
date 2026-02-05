# IS 362 week 2 homework

**Martin Crabtree**
IS-362 Week 2
**Instructions:** Your week 2 assignment is to create a small Jupyter (IPython) Notebook about one aspect of data structures that you might find somewhat challenging, such as set comprehensions, or using the zip() function. Your Jupyter Notebook should include both code and some documentation, which should utilize Markdown. Your Jupyter Notebook should be hosted in GitHub; please provide a link in your assignment submission.

## The data structure challenge: How do you implement the equivalent of a C++/C# 2D array in Python?

It is possible to recreate the equivalent of a C++/C# 2D array using nested lists in Python. For example the syntax for a basic matrix would be:

nested_list = [
[1, 2, 3],
[4, 5, 6],
[7, 8, 9]
]

This matrix works well on a small scale, however as the dataset becomes larger nested lists aren't ideal due to the way they are stored in memory, in addition to limited computational support. In most cases a NumPy array or Pandas dataframe offers better efficiency and functionality. However, there are cases where Python works well to handle 2D data without needing to import an external library. One case is creating a map data structure using x & y coordinates stored as a tuple to be used as a key in a Python dictionary. Since a dictionary is a type of hash map, it is very efficient for accessing and updating data. Also a dictionary works around issues with inefficient memory addressing found in a nested list, especially if the dataset contains empty data. As an added bonus a dictionary can easily check to see if a coordinate is within the map - avoiding "index out of range" errors.
