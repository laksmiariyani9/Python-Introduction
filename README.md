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

- Tuple
  - In Python, a tuple is a collection data type that is ordered and immutable. This means once a tuple is created, you cannot change its content (i.e., you cannot add, remove, or modify elements). Tuples are defined by enclosing comma-separated values within parentheses (). Here's a basic example of a tuple:
    - CODE
    - Tuples can contain elements of different data types, including integers, floats, strings, and even other tuples. For example:
  - Key Features of Tuples:
    - Ordered: Tuples maintain the order of elements as they are added.
    - Immutable: Once a tuple is created, its contents cannot be changed. This means you cannot add, remove, or modify elements in a tuple.

- Range
  - In Python, the range data type represents an immutable sequence of numbers. It is commonly used for iterating over a sequence of numbers in loops, particularly in for loops. The range type generates numbers on-the-fly, rather than storing them all in memory, making it memory efficient for large ranges.
  - The syntax for creating a range object is:
    - range(start, stop, step)
      - start: The starting value of the range (inclusive). If omitted, it defaults to 0.
      - stop: The ending value of the range (exclusive). This is the first value that is not included in the range.
      - step: The increment (or decrement if negative) between each number in the range. If omitted, it defaults to 1.
        
- Set
  - In Python, a set is a collection data type that is unordered, mutable, and contains unique elements. Sets are defined by enclosing comma-separated values within curly braces {}. Sets do not allow duplicate elements, and they automatically remove any duplicates when the set is created or modified. Here's a basic example of a set:
    - CODE
  - Sets can contain elements of different data types, including integers, floats, strings, and even tuples. For example:
    - CODE
  - Key Features of Sets:
    - Unordered: Sets do not maintain the order of elements as they are added.
    - Mutable: You can add or remove elements from a set after it is created.
    - Unique Elements: Sets do not allow duplicate elements. If you try to add a duplicate element to a set, it will be ignored.

- Frozenset
  - In Python, the frozenset data type is similar to the set data type, but with one key difference: it is immutable. This means that once a frozenset object is created, its contents cannot be changed.
  - Frozenset objects are useful when you need to create a collection of unique, immutable elements. They are particularly handy when you need to use sets as keys in dictionaries or as elements in other sets, as sets themselves are not hashable (mutable), but frozensets are hashable (immutable).
  - Here's how you create a frozenset object:
    - my_frozenset = frozenset({1, 2, 3, 4, 5})
  - You can also create a frozenset from other iterables like lists or tuples:
    - my_frozenset = frozenset([1, 2, 3, 4, 5])
    - my_frozenset = frozenset((1, 2, 3, 4, 5))

- Bytes
  - In Python, the bytes data type represents a sequence of bytes. Bytes objects are immutable, meaning they cannot be changed after creation. They are commonly used for handling binary data, such as reading from or writing to files, working with network protocols, and interacting with low-level system interfaces.
  - You can create a bytes object by enclosing a sequence of bytes within a pair of single quotes (b'') or double quotes (b""). Here's an example:
    - my_bytes = b'hello'
      - In this example, my_bytes is a bytes object containing the ASCII-encoded bytes representing the string "hello".
  - Bytes objects support various operations and methods for working with binary data, including:
    - Indexing: Accessing individual bytes using index notation.
      - CODE
    - Slicing: Extracting a portion of the bytes object.
      - CODE
    - Length: Getting the length of the bytes object.
      - CODE
    - Converting to String: Converting the bytes object to a string using decoding.
      - CODE
    - Concatenation: Combining two bytes objects.
      - CODE

- Bytearray
  - In Python, the bytearray data type is similar to the bytes data type, but with one key difference: it is mutable. This means that a bytearray object can be modified after it is created, whereas a bytes object is immutable and cannot be changed.
  - A bytearray object represents a sequence of bytes and is commonly used for situations where you need to modify binary data in place, such as reading from or writing to files, working with network protocols, or performing low-level system interactions.
  - You can create a bytearray object by passing a sequence of bytes to the bytearray() constructor. Here's an example:
    - my_bytearray = bytearray(b'hello')
      - In this example, my_bytearray is a bytearray object containing the ASCII-encoded bytes representing the string "hello".
  - Bytearray objects support various operations and methods for working with binary data, including:
    - Indexing: Accessing individual bytes using index notation.
      - CODE
    - Slicing: Extracting a portion of the bytearray object.
      - CODE
    - Length: Getting the length of the bytearray object.
      - CODE
    - Modifying Bytes: Changing the value of bytes in the bytearray object.
      - CODE
    - Appending Bytes: Adding new bytes to the end of the bytearray object.
      - CODE

- Memoryview
  - In Python, the memoryview data type provides a way to access the internal data of an object that supports the buffer protocol. It allows you to view the memory of an object without making a copy of it. This can be particularly useful when working with large amounts of data or when you want to avoid unnecessary memory duplication.
  - The memoryview object acts as a view into the memory of another object, such as a bytes, bytearray, or even a list. It allows you to access and manipulate the underlying data using slicing, indexing, and other operations.
  - You can create a memoryview object by passing an object that supports the buffer protocol to the memoryview() constructor. Here's an example:
    - my_bytes = b'hello'
    - my_memoryview = memoryview(my_bytes)
      - In this example, my_memoryview is a memoryview object that provides a view into the memory of the my_bytes object.
  - Memoryview objects support various operations and methods for accessing and manipulating the underlying data, including:
    - Indexing: Accessing individual elements using index notation.
      - CODE
    - Slicing: Extracting a portion of the memoryview object.
      - CODE
    - Length: Getting the length of the memoryview object.
      - CODE
    - Conversion to Bytes: Converting the memoryview object to bytes.
      - CODE
    - Accessing Buffer Info: Getting information about the underlying buffer.
      - CODE

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

- NoneType
  - In Python, NoneType is a data type that has only one value: None. It represents the absence of a value or a null value. None is commonly used to indicate that a variable or an expression doesn't have a meaningful value or hasn't been assigned a value yet.
  - Here's an example of how None is used:
    - my_variable = None
      - In this example, my_variable is assigned the value None, indicating that it doesn't currently have a meaningful value.
  - None is often used in conditional statements to check whether a variable has been assigned a value or not. For example:
    - CODE
      - In this example, the calculate_something() function returns None if it encounters an error or if the result is not available. The code checks whether the result is None before proceeding with further processing.
  - It's important to note that None is not the same as False, 0, an empty string '', or an empty list []. Those values represent specific values (false, zero, empty string, empty list) whereas None represents the absence of any value.

## PYTHON LOOPS
  - In Python, a loop is a programming construct that allows you to execute a block of code repeatedly. There are two main types of loops in Python: for loops and while loops.
    - For Loop: A for loop is used for iterating over a sequence (such as a list, tuple, string, or range) and executing a block of code once for each element in the sequence. The general syntax of a for loop is:
      - CODE
        - Here, 'item' is a variable that takes the value of the next element in the sequence on each iteration.
      - Example:
        - CODE
    - While Loop: A while loop is used to repeatedly execute a block of code as long as a specified condition is true. The general syntax of a while loop is:
      - CODE
        - The loop continues to execute as long as the condition remains True. If the condition becomes False, the loop terminates.
          

## PYTHON OPERATORS
  - In Python, operators are special symbols or keywords used to perform operations on variables and values. Python supports various types of operators, which can be categorized into the following groups:
    - Arithmetic Operators: These operators are used to perform arithmetic operations such as addition, subtraction, multiplication, division, modulus, and exponentiation. Here are the arithmetic operators in Python:
        - + (Addition)
        - - (Subtraction)
        - * (Multiplication)
        - / (Division)
        - % (Modulus)
        - ** (Exponentiation)
        - // (Floor Division)
      - Arithmetic Operators Syntax:
        - CODE
      - Example
        - CODE
          
  - Comparison (Relational) Operators: These operators are used to compare values. They return either True or False based on the comparison result. Here are the comparison operators:
        - == (Equal to)
        - != (Not equal to)
        - < (Less than)
        - > (Greater than)
        - <= (Less than or equal to)
        - >= (Greater than or equal to)
      - Comparison (Relational) Operators Syntax:
        - CODE
      - Example
        - CODE


## UNION
  - In set theory, the union of two sets is a new set that contains all the distinct elements from both sets.
  - In Python, you can perform these operations using the built-in set data type and its methods:
    - CODE
      

## INTERSECTION
  - The intersection of two sets is a new set containing only the elements that are common to both sets.
  - In Python, you can perform these operations using the built-in set data type and its methods:
    - CODE

## DICTIONARY
  - A dictionary in Python is an unordered collection of items. Each item in a dictionary is stored as a key-value pair.
  - Keys are unique within a dictionary while values may not be unique.
  - Dictionary elements can be accessed by their keys rather than their index as in lists.
  - Here's an example of a dictionary:
    - CODE

## Slicing
  - In Python, slicing is a technique used to extract a portion (or a slice) of a sequence-like data type such as strings, lists, tuples, etc. Slicing allows you to retrieve a subset of elements from the original sequence based on specified start and stop indices.
  - The syntax for slicing in Python is:
    - CODE
      - start: The index representing the beginning of the slice (inclusive). If omitted, slicing starts from the beginning of the sequence.
      - stop: The index representing the end of the slice (exclusive). If omitted, slicing goes until the end of the sequence.
      - step: The step size used to skip elements. If omitted, the default value is 1.
