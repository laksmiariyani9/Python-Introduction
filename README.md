# THE FUNDAMENTALS OF PYTHON 

## PYTHON DATA TYPES
A data type is an attribute associated with a piece of data that tells a computer system how to interpret its value. Python Data Types are used to define the type of a variable. It defines what type of data we are going to store in a variable. The data stored in memory can be of many types.
- Number
  - In Python, the "number type" refers to the data types used to represent numeric values. There are several numeric data types in Python:
    - Integer (int): Represents whole numbers without any decimal point. For example, 5, -10, 100, etc.
    - Floating-point (float): Represents numbers with a decimal point or in exponential form. For example, 3.14, -0.001, 2.71828, etc.
    - Complex: Represents complex numbers with real and imaginary parts. It's represented as a + bj, where a and b are floats and j is the imaginary unit (sqrt(-1)). For example, 2 + 3j, -1 - 2j, etc.
      
- String
  - In Python, the string data type (str) is used to represent textual data. Strings are sequences of characters enclosed within either single quotes (') or double quotes ("). For example:
      - CODE
  - Strings can contain letters, numbers, symbols, and whitespace characters. They support various operations and methods for manipulation and formatting. 
   
- Boolean
  - In Python, the boolean data type (bool) represents truth values. There are only two boolean values: True and False. Booleans are used to make logical decisions and comparisons in programming.
    - Boolean values are commonly the result of comparison operations or logical operations. For example:
      - CODE
    - Boolean values are often used in conditional statements (if, elif, else) to control the flow of a program based on certain conditions. For example:
      - CODE
    - Boolean values can also be the result of logical operations such as and, or, and not. For example:
      - CODE
  
- List
  - In Python, the list data type (list) is used to store a collection of items. Lists are ordered, mutable (modifiable), and allow duplicate elements. They are defined by enclosing a comma-separated sequence of items within square brackets [].
    - For example:
      - CODE
  - Lists can contain elements of different data types, including integers, floats, strings, and even other lists.
  
- Slicing
  - In Python, slicing is a technique used to extract a portion (or a slice) of a sequence-like data type such as strings, lists, tuples, etc. Slicing allows you to retrieve a subset of elements from the original sequence based on specified start and stop indices.
  - The syntax for slicing in Python is:
    - CODE
      - start: The index representing the beginning of the slice (inclusive). If omitted, slicing starts from the beginning of the sequence.
      - stop: The index representing the end of the slice (exclusive). If omitted, slicing goes until the end of the sequence.
      - step: The step size used to skip elements. If omitted, the default value is 1.

- Tuple
  - In Python, a tuple is a collection data type that is ordered and immutable. This means once a tuple is created, you cannot change its content (i.e., you cannot add, remove, or modify elements). Tuples are defined by enclosing comma-separated values within parentheses (). Here's a basic example of a tuple:
    - CODE
    - Tuples can contain elements of different data types, including integers, floats, strings, and even other tuples. For example:
  - Key Features of Tuples:
    - Ordered: Tuples maintain the order of elements as they are added.
    - Immutable: Once a tuple is created, its contents cannot be changed. This means you cannot add, remove, or modify elements in a tuple.

- Set
  - In Python, a set is a collection data type that is unordered, mutable, and contains unique elements. Sets are defined by enclosing comma-separated values within curly braces {}. Sets do not allow duplicate elements, and they automatically remove any duplicates when the set is created or modified. Here's a basic example of a set:
    - CODE
  - Sets can contain elements of different data types, including integers, floats, strings, and even tuples. For example:
    - CODE
  - Key Features of Sets:
    - Unordered: Sets do not maintain the order of elements as they are added.
    - Mutable: You can add or remove elements from a set after it is created.
    - Unique Elements: Sets do not allow duplicate elements. If you try to add a duplicate element to a set, it will be ignored.

- Dictionary
  - In Python, a dictionary is a collection data type that is unordered, mutable, and consists of key-value pairs. Dictionaries are defined by enclosing comma-separated key-value pairs within curly braces {}. Each key-value pair is separated by a colon :. Here's a basic example of a dictionary:
    - CODE
      - In this example:
        - 'name', 'age', and 'city' are keys.
        - 'Alice', 30, and 'New York' are the corresponding values associated with those keys.
  - Key Features of Dictionaries:
    - Unordered: Dictionaries do not maintain the order of key-value pairs as they are added.
    - Mutable: You can add, remove, or modify key-value pairs in a dictionary after it is created.
    - Unique Keys: Keys in a dictionary must be unique. If you try to add a duplicate key, it will overwrite the existing value associated with that key.
