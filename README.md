Experiment No. 5

Name: Pranav Menon

PRN No.: 25070123085

Batch: ENTC - B1

Aim:

To study Dictionaries in Python and understand dictionary operations, methods, and their practical applications.

THEORY

1) Introduction to Dictionaries

A dictionary in Python is an ordered collection of key‑value pairs. Each key maps to a specific value, making dictionaries ideal for fast lookups and structured data storage. Dictionaries are defined using curly braces {} with the key:value syntax.

Key Characteristics:
• Ordered – Since Python 3.7, dictionaries preserve insertion order.
• Mutable – Keys and values can be modified after creation.
• Key‑Value Pairs – Data stored as associations between keys and values.
• Unique Keys – Duplicate keys are not allowed; the last value overwrites the previous one.
• Keys must be immutable types (e.g., strings, numbers, tuples).

Syntax:
my_dict = {"key1": value1, "key2": value2, "key3": value3}
OR
my_dict = dict(key1=value1, key2=value2, key3=value3)

2) Creating Dictionaries

Dictionaries can be created using curly braces with key:value pairs or the dict() constructor.

Example:
thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}

3) Accessing Dictionary Values

Values are accessed using their keys:
- Square bracket notation: dict[key]
- get() method: dict.get(key, default_value)

Example:
thisdict["brand"]        # Returns "Ford"
thisdict.get("brand")    # Returns "Ford"

The get() method is safer because it returns None or a default value if the key does not exist, while square brackets raise a KeyError.

4) Duplicate Keys Behavior

Dictionaries do not allow duplicate keys. If a key is repeated, the last value overwrites earlier ones.

Example:
thisdict = {"year": 1964, "year": 2020}
Result: {"year": 2020}

5) Dictionary Length

The len() function returns the number of key‑value pairs.

Example:
len(thisdict)   # Returns count of unique keys

6) Adding and Modifying Elements

New key‑value pairs can be added or existing values modified using square bracket assignment.

Example:
dict["newkey"] = "newvalue"   # Adds new pair
dict["year"] = 2025           # Updates existing value

7) Dictionary Methods

Common methods:
- keys() → Returns all keys
- values() → Returns all values
- items() → Returns key‑value pairs as tuples
- get(key, default) → Safe retrieval
- pop(key) → Removes and returns value for specified key
- update(dict2) → Merges another dictionary

8) Removing Elements

Elements can be removed using:
- pop(key) → Removes specified key and returns its value
- popitem() → Removes and returns the last inserted key‑value pair

Example:
student = {"roll": 101, "name": "Amit", "Branch": "ENTC"}
student.pop("Branch")

9) Membership Testing

The 'in' keyword checks if a key exists:
- "key" in dict → True if key exists
- "key" not in dict → True if key does not exist

10) Dictionary Type

The type() function confirms that dictionary objects belong to <class 'dict'>.

Example:
type(thisdict)   # Returns <class 'dict'>

ALGORITHMS

Algorithm 1: Updating Product Prices

Step 1: Start
   - Begin the process of updating product prices

Step 2: Initialize product dictionary
   - Command: Product = {"Pen": 10, "Book": 50, "Scale": 20}
   - Function: Dictionary creation using curly braces {}
   - Source: Built-in Python dictionary data structure (no import required)

Step 3: Display original product dictionary
   - Command: print("Original Product Dictionary : ", Product)
   - Function: print() - Built-in function for console output
   - Source: Built-in Python function (no import required)

Step 4: Update product price using key assignment
   - Command: Product["Book"] = 55
   - Function: Square bracket assignment - Modifies value for existing key
   - Source: Built-in dictionary operation (no import required)

Step 5: Display updated product dictionary
   - Command: print("Updated Product Dictionary : ", Product)
   - Function: print() - Built-in function for console output
   - Source: Built-in Python function (no import required)

Step 6: Stop
   - End the algorithm


Algorithm 2: Safe Student Marks Retrieval

Step 1: Start
   - Begin the process of retrieving student marks safely

Step 2: Initialize student marks dictionary
   - Command: Student = {"A": 92, "B": 82, "C": 72}
   - Function: Dictionary creation using curly braces {}
   - Source: Built-in Python dictionary data structure (no import required)

Step 3: Display original student dictionary
   - Command: print("Original Student Dictionary : ", Student)
   - Function: print() - Built-in function for console output
   - Source: Built-in Python function (no import required)

Step 4: Get student name from user
   - Command: name = input("Enter the Name of the Student : ")
   - Function: input() - Built-in function for user input
   - Source: Built-in Python function (no import required)

Step 5: Retrieve marks using get() method with default value
   - Command: Student.get(name, "Student Not Found")
   - Function: get(key, default) - Built-in dictionary method for safe retrieval
   - Source: Built-in dictionary method (no import required)

Step 6: Display the result
   - Command: print(Student.get(name, "Student Not Found"))
   - Function: print() - Built-in function for console output
   - Source: Built-in Python function (no import required)

Step 7: Stop
   - End the algorithm

Algorithm 3: User Login Authentication

Step 1: Start
   - Begin the process of user authentication

Step 2: Initialize users dictionary
   - Command: users = {"admin": "1234", "student": "abcd"}
   - Function: Dictionary creation using curly braces {}
   - Source: Built-in Python dictionary data structure (no import required)

Step 3: Get username from user
   - Command: username = input("Enter the Username : ")
   - Function: input() - Built-in function for user input
   - Source: Built-in Python function (no import required)

Step 4: Get password from user
   - Command: password = input("Enter the Password : ")
   - Function: input() - Built-in function for user input
   - Source: Built-in Python function (no import required)

Step 5: Check if username exists in dictionary
   - Command: if username in users:
   - Function: in - Membership operator for dictionary keys
   - Source: Built-in Python operator (no import required)
     
Step 6: Verify password for valid username
   - Command: if users[username] == password:
   - Function: Square bracket access and == comparison operator
   - Source: Built-in Python operators (no import required)

Step 7: Display login successful message
   - Command: print("Login Successful")
   - Function: print() - Built-in function for console output
   - Source: Built-in Python function (no import required)

Step 8: Display login unsuccessful message
   - Command: else: print("Login Unsuccessful ! Please Try Again")
   - Function: print() - Built-in function for console output
   - Source: Built-in Python function (no import required)

Step 9: Stop
   - End the algorithm

Algorithm 4: Finding Class Topper

Step 1: Start
   - Begin the process of finding class topper

Step 2: Initialize marks dictionary
   - Command: marks = {"A": 85, "B": 92, "C": 65}
   - Function: Dictionary creation using curly braces {}
   - Source: Built-in Python dictionary data structure (no import required)

Step 3: Display original marks dictionary
   - Command: print("Original Marks Dictionary : ", marks)
   - Function: print() - Built-in function for console output
   - Source: Built-in Python function (no import required)
     
Step 4: Find student with maximum marks
   - Command: topper = max(marks, key=marks.get)
   - Function: max() - Built-in function that returns maximum value
   - Source: Built-in Python function (no import required)

Step 5: Display topper name
   - Command: print("Topper of the Class : ", topper)
   - Function: print() - Built-in function for console output
   - Source: Built-in Python function (no import required)

Step 6: Display topper's marks
   - Command: print("Marks of the topper is : ", marks[topper])
   - Function: Square bracket access and print()
   - Source: Built-in Python operations (no import required)

Step 7: Stop
   - End the algorithm

Conclusion :
The study of Dictionaries in Python was successfully completed
