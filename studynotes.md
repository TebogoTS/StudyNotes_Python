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

Functional programming is a style of writing code that focuses on using functions as the main building blocks of a program. In this style, functions behave like mathematical functions: they take inputs, perform some operations, and produce outputs without changing or modifying any data outside their scope.

Think of functional programming as a set of actions, almost like a recipe of formula, where each action (function) takes something in, does something specific, and gives you something back without messing with other thngs around it.

### Example of functional programming
```
def square(x):
    return x * x

numbers = [1, 2, 3, 4, 5]

squared_numbers = list(map(square, numbers))
print(squared_numbers)
```

# Object-Oriented Programming (OOP):

Imagine you're building something with LEGO blocks. Each LEGO piece is like an object, and you can connect these pieces together to create somehting bigger, like a house or a car. In OOP, objects are like these LEGO pieces, and you use them to build larger and more complex structures.

### Key Concepts in OOP:

1. <b>Objects:<b> Objects are the basic building blocks of OOP. They represent real-world things and contain both data (attributes) and actions (methods/functions).
2. Classes: Classes are like blueprints or templates that define how an object will look and behave. They encapsulate the behavior and properties common to a group of objects.
3. Encapsulation: This means bundling the data (attributes) and the methods (functions) that operate on the data into a single unit (an object).
4. Inheritance: Objects can inherit properties and behavior from other objects. For example, a "Car" object can inherit features from a more general "Vehicle" class.
5. Polymorphism: This refers to the ability of different objects to be treated as objects of a common type. For instance, a "Circle" object and a "Rectangle" object can both be treated as "Shapes" because they share certain characteristics.