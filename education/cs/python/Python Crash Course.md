
This will contain any important info derived from my time reading through the book: 
'Python Crash Course, 3rd Edition'

##### Important Notes:

- Simple is better than complex.
- Complex is better than complicated.
- Readability is important.

- When changing attributes within functions, remember to recall the function to see the changed output, else it will appear as though it hasn't changed when it has.

##### Variables:

- Can contain letters, underscores, or numbers, but can only start with a letter, else this will throw an error.
- Variable names must be abstract, meaning they cannot be the same as an existing word reserved for a particular Python function, eg: 'print' is a word that shouldn't be used in a variable name.
- Variables can be overridden and reassigned.

##### Traceback:

- A traceback is a record of where the interpreter found the error, and it gives an error message based on the type of error.

#### Lists:

- Lists are dynamic, meaning they can be added to and have values removed at any time.
- Indentation is important in ensuring correct output.
- If the code has correct syntax, but produces an undesired result, this is a 'logical' error.

#### The if-elif-else chain:

When using if functions, it is typical to use if, followed by elif, and then else, if more than two arguments are being used. Otherwise it would be if, else.


#### Flags:

Flags can be used to enter and exit loops, to collect information etc, and then exit the loop.

An example would be: 

```python

vacation = {}

  

polling_active = True

  

while polling_active:

    name = input("What is your name? ")

    response = input("What country would you like to go on vacation to? ")

  

    vacation[name] = response

  

    repeat = input("Should another person respond? ")

    if repeat == 'No':

        polling_active = False
```


#### Functions:

Functions are a key part of programming in python, they allow for code to be organised by having information and tasks inside. They can be used to input and output information, and are a fundamental concept used in professional settings.

Functions allow for code to be written, and then reused, eliminating the need to rewrite any existing code.

#### Inheritance:

Inheritance is when one class 'inherits' from another, this can be used to reduce unnecessary code by reusing variables, which is especially useful in large codebases. When inheritance is used, the class being inherited from would become the parent, and the one inheriting would become a child of that parent.

```Python

class Car():

	 def __init__(self, make, model, year):        
	 self.make = make        
	 self.model = model        
	 self.year = year        
	 self.odometer_reading = 0
	 
class ElectricCar(Car):

```
For this example. Car would be the parent, and ElectricCar the child as it inherits the 'Car' class.

#### Instances as Attributes:

Classes can be broken down into smaller classes in order to reduce code bloat, this is important in large codebases, for example, related functions could be broken down into one subclass, rather than all being in the main parent class.

