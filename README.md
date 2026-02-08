Experiment No. 5

Name: Pranav Menon

PRN No.: 25070123085

Batch: ENTC - B1

Aim:

To study Dictionaries in Python and understand dictionary operations, methods, and their practical applications.

THEORY

1) Introduction to Dictionaries

A dictionary is an ordered collection of key-value pairs in Python. Dictionaries are defined using curly braces {} with key:value syntax.

Key Characteristics:

• Ordered - Maintains insertion order (Python 3.7+)

• Mutable - Keys and values can be modified after creation

• Key-Value Pairs - Data stored as key:value associations

• Unique Keys - Duplicate keys are not allowed; last value overwrites previous

Syntax:

my_dict = {"key1": value1, "key2": value2, "key3": value3}
OR
my_dict = dict(key1=value1, key2=value2, key3=value3)

2) Creating Dictionaries

Dictionaries can be created using:
- Curly braces with key:value pairs
  
Example:
thisdict = {"brand": "Ford", "model": "Mustang", "year": 1964}

3) Accessing Dictionary Values

Values can be accessed using:
- Square bracket notation: dict[key]
- get() method: dict.get(key, default_value)

Example:
thisdict["brand"]  # Returns "Ford"
thisdict.get("brand")  # Returns "Ford"

The get() method is safer as it returns None or a default value if key doesn't exist, while square brackets raise KeyError.

4) Duplicate Keys Behavior

Dictionaries do not allow duplicate keys. If a key is repeated during creation or assignment, the last value associated with that key will overwrite all previous values.

Example:
thisdict = {"year": 1964, "year": 2020}
Result: {"year": 2020}  # First value (1964) is overwritten

5) Dictionary Length

The len() function returns the number of key-value pairs in a dictionary.

Example:
len(thisdict)  # Returns count of unique keys

6) Adding and Modifying Elements

New key-value pairs can be added or existing values can be modified using:
- Square bracket assignment: dict[key] = value

If key exists: value is updated
If key doesn't exist: new key-value pair is added

7) Dictionary Methods

Common methods:
- keys() - Returns all keys
- values() - Returns all values  
- items() - Returns key-value pairs as tuples
- get(key, default) - Safe value retrieval
- pop(key) - Removes and returns value for specified key
- update(dict2) - Merges another dictionary

8) Removing Elements

Methods for removal:
- pop(key) - Removes specified key and returns its value; raises KeyError if key not found
- popitem() - Removes and returns last inserted key-value pair

student = {
    "roll" : 101,
    "name" : "Amit",
    "Branch" : "ENTC",
}
student.pop("Branch")

9) Membership Testing

The 'in' keyword checks if a key exists in dictionary:
- "key" in dict - Returns True if key exists
- "key" not in dict - Returns True if key doesn't exist

10) Dictionary Type

The type() function returns <class 'dict'> for dictionary objects.

Example:
type(thisdict)  # Returns <class 'dict'>

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
