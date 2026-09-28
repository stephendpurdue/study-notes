
#### What is it?

Reading from files simply means opening an external file and using the information inside, this could be as simple as printing it.

#### Example:

```Python
with open('hello.py') as file_object: # Opens and then closes the file
	contents = file_object.read() # Creates a variable and reads the contents
	print(contents) # Prints the variable 
```

#### Best Practices:

One of the main best practices is to use 'with open' when opening a file, and not to use close(). This prevents issues with opening and closing which can lead to data corruption and working with a closed file.


#### Methods:

There are three main methods when reading files: reading, writing, and appending.

- Reading will simply read the file
- Writing will add new content, but overwrite any existing content
- Appending will add to the file without overwriting the existing content.

Unless explicitly needing to remove the main content, it's best to use .append in order to prevent unexpected losses.

Multiple files can be read at once by putting their names in a list, looping through the list, and then printing the results.