
#### What are Classes?

Classes are used to organise code and ensure efficiency across a codebase. They take methods in order to run. Classes work by taking in attributes, these are then used in methods (functions), and are then called at the end using dot notation. A clearer explanation is that classes can be thought of as blueprints, they are used to scaffold data and make it cleaner and more usable.

#### How do we use Classes?

Class are used from the 'class' syntax, followed by the name of the class and '():'
To declare attributes, classes typically have a constructor, followed by variables.

```Python

class Car():

	def __init__(self, make, model, year):
		self.make = make
		self.model = model
		self.year = year
		
	def describe_car(self): # This is an instance (an object built from the class)
		print("This car is a " + self.make + 
		" " + self.model + " and it was made in " 
		+ str(self.year))
		  
		  
		  
my_car = Car('BMW', 'A1', 2019)
print(my_car)
```
This example starts with a constructor, which takes in three variables, these variables are declared in the constructor using self. followed by the name. These store them and make them usable. A function is then used combining all the variables into a printed string.

Under the hood, classes work by allocating a new object in memory, calling the constructor, using self to bind an attribute onto an object, eg: 'self.make = make'. The object is then returned and made assignable.


#### Why do we use Classes?

Classes are used to make creating programs easier, especially in large codebases. It allows for specific functions to be kept assigned to specific classes, helping to avoid conflicts.

It also allows for high reusability, making functions quick to import and use elsewhere in a codebase.

#### Best Practices:

Classes should be written in CamelCaps, and without underscores. This means that the first letter of each word in the class name should be capitalised.
There should also be a docstring or comment next to the class to document what it does and why.

#### Importance:

Classes are the backbone of Object Oriented Programming, and essential in most industry settings.



