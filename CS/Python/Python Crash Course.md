
This will contain any important info derived from my time reading through the book: 
'Python Crash Course, 3rd Edition'

##### Important Notes:

- Simple is better than complex.
- Complex is better than complicated.
- Readability is important.

##### Variables:

- Can contain letters, underscores, or numbers, but can only start with a letter, else this will throw an error.
- Variable names must be abstract, meaning they cannot be the same as an existing word reserved for a particular Python function, eg: 'print' is a word that shouldn't be used in a variable name.

##### Traceback:

- A traceback is a record of where the interpreter found the error, and it gives an error message based on the type of error.

#### Lists:

- Lists are dynamic, meaning they can be added to and have values removed at any time.
- Indentation is important in ensuring correct output.
- If the code has correct syntax, but produces an undesired result, this is a 'logical' error.

#### The if-elif-else chain:

When using if functions, it is typical to use if, followed by elif, and then else, if more than two arguments are being used. Otherwise it would be if, else.


#### Flags:

Flags can be used to enter and exit loops, and to collect information etc, and then exit the loop.

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


