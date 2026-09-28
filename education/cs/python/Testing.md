
#### What is Unit Testing?

Testing involves adding unit tests to ensure functions work as expected.

This can be done by importing the 'unittests' module, it is best to do this in a separate file to reduce clutter.

#### Assert Methods:

An assert method is available in the unittest module, and are used to verify return values are as expected.

- assertEqual(a, b) -> Verify that a == b
- assertNotEqual(a, b) -> Verify that a != b
- assertTrue(x) -> Verify that x is True
- assertFalse(x) -> Verify that x is False
- assertIn(item, list) -> Verify that an item is in a list
- assertNotIn(item, list) -> Verify that an item is not in a list

#### Example:

``` 
import unittest # Imports the module
from calculator import Calculator # Imports the class we are testing

class TestCalculator(unittest.TestCase): # Defines the core class for tests

    def test_addition(self): # Tests the addition function
        calc = Calculator() # Sets the class as a usable variable
        result = calc.add(17, 20) # Does a test calculation
        self.assertEqual(result, 37) # Sets this as the correct calculation

    def test_subtraction(self):
        calc = Calculator()
        result = calc.subtract(20, 10)
        self.assertEqual(result, 10)

    def test_multiplication(self):
        calc = Calculator()
        result = calc.multiply(5, 5)
        self.assertEqual(result, 25)

    def test_division(self):
        calc = Calculator()
        result = calc.divide(10, 5)
        self.assertEqual(result, 2)

if __name__ == "__main__":
	unittest.main()
```

This is a very simple example created for a small calculator app.

#### Notes:

One mistake I kept making was putting the arguments in the self.assertEqual method. This is wrong, it's supposed to be the correct outcome, not the arguments again. If testing strings, using an f string is a good idea to ensure different inputs are accepted.


