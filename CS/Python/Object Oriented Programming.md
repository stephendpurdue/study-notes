
### DRY Principle:

The dry principle is extremely simple: 'don't repeat yourself'. Use unique and descriptive names for variables, functions, and classes, and don't write unnecessary code, or duplicate code, if an existing code segment can be added to or refactored rather than re-written, this is preferrable.

### Classes:

Classes are used to organise code and ensure efficiency across a codebase. They take methods in order to run. 

#### Dot Notation:

Dot notation is used when accessing the value of an attribute. For example, the dot notation seen here is when accessing the age or name of the cat.

```Python

class Cat():

    def __init__(self, name, age):

        self.name = name

        self.age = aga
  
    def sit(self):

        print(self.name.title() + " is now sitting.")

    def roll_over(self):

        print(self.name.title() + " rolled over!")

my_cat = Cat('Mo Mo', 13)

  

print("My cat's name is  " + my_cat.name.title() + ".")
print("My cat is " + str(my_cat.age) + " years old.")
	
```

