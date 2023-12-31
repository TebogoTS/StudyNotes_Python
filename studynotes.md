# Procedural Programming

Procedural programming is a paradigm in which the program's structure is based on procedures or functions that perform specific tasks.

# Example of procedural programming
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

result = add(5, 3)
print(result)

result = subtract(10, 4)
print(result)

# Functional Programming

Functional programming emphasizes the use of functions that produce outputs based on inputs without changing state or data.

# Example of functional programming
def square(x):
    return x * x

numbers = [1, 2, 3, 4, 5]

squared_numbers = list(map(square, numbers))
print(squared_numbers)
