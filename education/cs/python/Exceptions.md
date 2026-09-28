
Exceptions are pythons way of preventing crashes and bugs, it typically uses a 'try:' and 'except:' syntax, but can also use a 'try:', 'except:', 'else:' syntax, which will perform the intended operation if no error is thrown.

#### Example:

```Python
  

while True:

    first_number = input("\nFirst Number: ")

    if first_number == 'q':

        break

    second_number = input("\nSecond Number: ")

    if second_number == 'q':

        break

    try:

        answer = int(first_number) * int(second_number)

    except ZeroDivisionError:

        print("You can't multiply by zero!")

    else:    

        print(answer)
```
In this example, two numbers are asked for, and then multiplied, the program is looking for two things: if 'q' is pressed (this will exit the program) or if a number is entered, which will continue the program. This is following the try, except, else chain.

