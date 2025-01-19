# Vs.code.py 

#Basics Evrey new python user should know
# Variables and Data Types
name = "John Doe"
age = 30
is_adult = True

print("Name:", name)
print("Age:", age)
print("Is Adult:", is_adult)

# Lists
fruits = ["apple", "banana", "cherry"]
print("Fruits:", *fruits)

# Loops
for fruit in fruits:
    print(fruit)

# Conditional Statements
if age > 18:
    print("You are an adult")
else:
    print("You are not an adult")

# Functions
def greet(name):
    print("Hello, " + name)

greet("John")

# Classes and Objects
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def greet(self):
        print("Hello, my name is " + self.name + " and I am " + str(self.age) + " years old")

person = Person("John Doe", 30)
person.greet()

# Tuples
colors = ("red", "green", "blue")
print("Colors:", colors)

# Dictionaries
person_info = {"name": "John Doe", "age": 30}
print("Person Info:", person_info)

# Sets
unique_colors = {"red", "green", "blue"}
print("Unique Colors:", unique_colors)

# Try-Except Blocks
try:
    print(5 / 0)
except ZeroDivisionError:
    print("Error: Division by zero is not allowed")

# Lambda Functions
double = lambda x: x * 2
print("Double of 5:", double(5))

# Map Function
numbers = [1, 2, 3, 4, 5]
squared_numbers = list(map(lambda x: x ** 2, numbers))
print("Squared Numbers:", squared_numbers)

# Filter Function
even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
print("Even Numbers:", even_numbers)

# List Comprehensions
squared_numbers = [x ** 2 for x in numbers]
print("Squared Numbers:", squared_numbers)

# Generators
def infinite_sequence():
    num = 0
    while True:
        yield num
        num += 1

gen = infinite_sequence()
print("Next Number:", next(gen))
print("Next Number:", next(gen))
print("Next Number:", next(gen))