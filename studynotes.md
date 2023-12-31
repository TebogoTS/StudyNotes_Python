# Procedural Programming

Procedural programming is a paradigm in which the program's structure is based on procedures or functions that perform specific tasks.

Procedural programming is a way of writing code where you break down your program into smaller, manageable chunks called procedures or functions. These functions are like individual steps or tasks that perform specific jobs within the program.

For example, imagine you're preparing a meal. You have various steps like chopping vegetables, cooking rice, frying chicken, etc. Each of these steps represents a procedure in the cooking process. Similarly, in procedural programming, you create functions that handle specific tasks like calculating, sorting, printing or any other action needed in your program.

### Example of procedural programming
```
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

result = add(5, 3)
print(result)

result = subtract(10, 4)
print(result)
```
### Example: A simple Python example demonstrating procedural programming.

##### Function to calculate the area of a rectangle
```
def calculate_area(length, width):
    return length * width
```
##### Function to display the area of a rectangle
```
def display_are(length, with):
    area = calculate_area(length, width)
    print(f"The area of the rectangle is: {area} square units.")
```
##### Main program
```
length = 5
width = 3
```
##### Call the function to display the area.
```
display_area(length, width)
```
# Functional Programming

Functional programming emphasizes the use of functions that produce outputs based on inputs without changing state or data.

### Example of functional programming
```
def square(x):
    return x * x

numbers = [1, 2, 3, 4, 5]

squared_numbers = list(map(square, numbers))
print(squared_numbers)
```