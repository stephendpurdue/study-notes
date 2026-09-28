
#### What is importing?

Importing is the act of importing outside information or data, this includes modules or libraries.

Importing a module can involve a package, file or library, a library is an outside tool to be used within python, such as PyTorch or PyGame.

Some modules and libraries are already built into python itself, such as 'random' and 'math'.

#### How do we import?

Importing can be done using the 'import' syntax, for example:

```Python

	from car import Car # Imports a specific class from the module.
	from car import ElectricCar # Imports a specific class from the module.
	from car import * # Imports all classes from the module. (Typically discouraged)
	from car import ElectricCar as EC # Imports a specific class as an alias.

```

Modules can be imported from files created, external sources, and collections.
#### Why do we import?

Importing is done to keep codebases tidy and remove code bloat, classes can be kept in their own files, and then imported to another when required, this ensures that each class is kept separate to ensure clarity and cleanliness.

This also helps to improve code reusability, by keeping separate from other classes, it can be reused easily.


#### Importance:

There aren't really any drawbacks to importing, however this can get a bit confusing across large codebases, so memorisation is key. However, one key drawback is namespace collisions, which happens when there are more than one thing with the same name -> avoid this!

#### Key Modules:

One key module comes from collections, and is included with each python installation, OrderedDict(). This connects pieces of information, and keeps them in their original order, this combines two features of lists and dictionaries.

#### Other Modules:

Pygal is a useful module that can be used to create structured bar graphs and data charts, it is similar to matplotlib, but designed more for bar graphs.
