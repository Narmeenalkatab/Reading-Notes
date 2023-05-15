# Reading Questions
## Explain the concept of variable scope in Python and describe the difference between local and global scope. Provide an example illustrating the usage of both.

variable scope refers to the region of a program where a variable can be accessed or referenced. Python has two types of variable scope: local and global. Local variables are defined inside a function or a block and can only be accessed within that function or block. Global variables, on the other hand, are defined outside of any function or block and can be accessed from anywhere in the program.


 ```
 #Global variable
name = "narmeen"

def greet():
    # Local variable
    message = "Hello"
    print(message + ", " + name)

greet()  # Output: Hello, narmeen
```




## How do the global and nonlocal keywords work in Python, and in what situations might you use them?

You would use these keywords when you want to modify a variable outside the current scope of a function, especially when working with nested functions.


## In your own words, describe the purpose and importance of Big O notation in the context of algorithm analysis.

Big O notation is a way of describing the efficiency of an algorithm by analyzing how the runtime or space requirements of the algorithm grow with the size of the input. It's a standardized way of comparing the performance of different algorithms and is important because it helps developers choose the most efficient algorithm for a given problem.



## Based on the Rolling Dice Example, explain how you would simulate a dice roll using Python. Describe how you would use code to calculate the probability of rolling a specific number (e.g., the probability of rolling a 6) over a large number of trials.

we can use the **random** module, which provides a randint function that generates a random integer within a specified range.

 simulates a dice roll example :
```
import random

def roll_dice():
    return random.randint(1, 6)

result = roll_dice()
print(result)  # Output: a random integer between 1 and 6

```

the probability of rolling a 6 example:
```
def calculate_probability(num_trials, target_num):
    count = 0
    for i in range(num_trials):
        if roll_dice() == target_num:
            count += 1
    return count / num_trials

probability = calculate_probability(10000, 6)
print(probability)  # Output: the probability of rolling a 6 over 10000 trials

```
