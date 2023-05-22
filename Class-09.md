# Read: Class 09


Reading Questions
What is the purpose of dunder methods in Python? Provide an example of a commonly used dunder method.

(it is a short for "double underscore" methods)
The purpose of dunder methods  in Python is to provide special behaviors and functionality to objects of a class. These methods are also known as magic methods or special methods. The name "dunder methods." Dunder methods are predefined and invoked implicitly in response to certain operations or actions on objects. They allow you to customize the behavior of built-in operations and operators, such as arithmetic operations, comparison operations, object creation, and more.

Ex:
 The __init__

 class MyClass:
    def __init__(self, name):
        self.name = name

obj = MyClass("narmeen")
print(obj.name)
Output: narmeen





In the video “AI Guru makes $238,800 with misleading paid course,” what was the main ethical issue raised concerning the use of developers’ work, and how might this have been avoided?

 statistics provides a framework and tools for analyzing and interpreting data, enabling researchers, analysts, and decision-makers to make sense of information, identify patterns, and draw meaningful conclusions.

Describe the Python statistics module and give an example of a function within the module that can be used to perform a common statistical operation.

 Python statistics module provides functions for performing various statistical operations and calculations. It includes functions for measures of central tendency, measures of dispersion, probability distributions, hypothesis testing, and more.

 Ex:
 mean() function is used to calculate the mean value


 import statistics

data = [1, 2, 3, 4, 5]
mean_value = statistics.mean(data)
print(mean_value)   Output: 3
