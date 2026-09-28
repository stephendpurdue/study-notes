
Matplotlib can be used to display and sort large amounts of data.

First, data is created or loaded, then, x and y values are defined and added to the graph. Labels can be used to name and organise data on the graph.

```# This creates a line graph showing square numbers from 1 -> 25.

x_values = list(range(1, 1001))

y_values = [x**2 for x in x_values] # X squared for each number in x_values
  

plt.scatter(x_values, y_values, c=y_values, edgecolor='none', s=10) # Plots the list

plt.show() # Initialises the viewer


# Labels


plt.title("Square Numbers", fontsize=24)

plt.xlabel("Value", fontsize=14)

plt.ylabel("Square of Value", fontsize=14)

plt.tick_params(axis='both', which='major', labelsize=14)


# Saving


plt.savefig('squares_plot.png', bbox_inches='tight')
```

In this code snippet, no data is loaded. x and y values are defined as a list of 1000 numbers, and cube numbers. These are then plotted against each other to see all the cube numbers between 1 and 1000. This is done using a for loop.

The data is then scattered across the graph and shown using the .show() command.

Labels are used here to define each set of data.
