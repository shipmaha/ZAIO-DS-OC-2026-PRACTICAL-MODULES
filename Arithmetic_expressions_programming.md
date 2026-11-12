Task 1: Arithmetic expressions in programming
Provide evidence, then save before moving on.

1.1 - Provide python 3 code for a function that takes in a list of numbers as an argument and returns the sum of only the positive numbers of the provided list. (5 marks)

def sum_positive(numbers):
    total = 0
    for num in numbers:
        if num > 0:
            total += num
    return total

1.2 - Provide python 3 code for a function that takes in a list of numbers as an argument and returns the product of all the numbers in the list. (5 mark)

def product(numbers):
    result = 1
    for num in numbers:
        result *= num
    return result

1.3 - Provide python 3 code for a function that takes in a radius as an argument and calculates the circumference of a circle. (5 marks)

import math

def circumference(radius):
    return 2 * math.pi * radius

1.4 - Provide python 3 code for a function that takes in area and base as arguments and calculates the height of a triangle. (5 marks)

def triangle_height(area, base):
    if base == 0:
        raise valueerror("Base cannot be zero.")
    return 2 * area / base
