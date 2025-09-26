## ToDo:
- ~~Python OOP Beginners - YouTube video - https://youtu.be/JeznW_7DlB0~~
- ~~Programming paradigm - Functional/Procedural/Object-oriented~~
- ~~Object-Oriented Programming (OOP) in Python - https://realpython.com/python3-object-oriented-programming/~~
- *Building **Library Management System** with Classes in Python*
- *Python Classes: The Power of Object-Oriented Programming - https://realpython.com/python-classes/*
- DuckTyping - Polymorphism - Abstract base classes (ABCs) ?
- ~~`objectA == objectB` => ? ; `objectA is objectB` => ?~~
- difference between `__new__()` and `__init__()` ?
- Python Class Constructors: Control Your Object Instantiation - https://realpython.com/python-class-constructor
- Providing Multiple Constructors in Your Python Classes - https://realpython.com/python-multiple-constructors/
- Python's Instance, Class, and Static Methods Demystified - https://realpython.com/instance-class-and-static-methods-demystified/
- Getters and Setters: Manage Attributes in Python - https://realpython.com/python-getter-setter/
- Python Error Handling - https://realpython.com/python-lbyl-vs-eafp/
- ~~Namespaces and Scope in Python - https://realpython.com/python-namespaces-scope/~~
- ~~How Do You Choose Python Function Names? - https://realpython.com/python-function-names/~~
- Data Classes in Python 3.7+ - https://realpython.com/python-data-classes/
- Build Enumerations of Constants With Python's Enum - https://realpython.com/python-enum/
- Write Pythonic and Clean Code With namedtuple - https://realpython.com/python-namedtuple/
- ~~The Zen of Python: `import this`~~
- Python Descriptors: An Introduction - https://realpython.com/python-descriptors/
- Python's property(): Add Managed Attributes to Your Classes - https://realpython.com/python-property/
- Python's Instance, Class, and Static Methods Demystified - https://realpython.com/instance-class-and-static-methods-demystified/
- Python's Magic Methods: Leverage Their Power in Your Classes - https://realpython.com/python-magic-methods/
- Build a Python Directory Tree Generator for the Command Line - https://realpython.com/directory-tree-generator-python/#coding-the-high-level-directorytree-class
- The most common tool for doing type checking is `mypy`. - https://mypy-lang.org/
- Getting Started With Testing in Python - https://realpython.com/python-testing/
- Python Code Quality: Best Practices and Tools - https://realpython.com/python-code-quality/
- How to Write Docstrings in Python - https://realpython.com/how-to-write-docstrings-in-python/
- Python Timer Functions: Three Ways to Monitor Your Code - https://realpython.com/python-timer/
- Python Metaclasses - https://realpython.com/python-metaclasses/
- Primer on Python Decorators - https://realpython.com/primer-on-python-decorators/
- Single and Double Underscores in Python Names - https://realpython.com/python-double-underscore
- Absolute vs Relative Imports in Python - https://realpython.com/absolute-vs-relative-python-imports/
- Data Classes in Python 3.7+ (Guide) - https://realpython.com/python-data-classes/

---

## Dump:
- Class
- Object or instance
- attributes
- methods
- dunder methods
- Class attributes
- Instance attributes
- Instance methods
- Class methods
- Static methods:
  > - You’ll typically define a static method instead of a regular function outside the class when that function is closely related to your class, and you want to bundle it together for convenience or for consistency with your code’s API.
  > - You should generally call static methods through the corresponding class instead of one of its instances.
- inheritance
- parent class
- child class
- Encapsulation
  > - A fundamental OOP principle that recommends protecting an object’s state or data from the outside world, preventing direct access.
  > - In Python, it’s completely normal to expose attributes as part of an object’s public API. If you ever need to add function-like behavior on top of a public attribute, then you can turn it into a property instead of breaking the API by replacing the attribute with a method.
- Inheritance
- Abstraction
- Polymorphism
- Public & Non-Public Members
- **Managed attributes:** Python allows you to add function-like behavior on top of existing instance attributes and turn them into managed attributes. To create a managed attribute with function-like behavior in Python, you can use either a property or a descriptor, depending on your specific needs.
- `__repr__()` method
- `__hash__()` method (hashability in class)
- protocols
- A single leading underscore, such as with `_foo()`, to indicate that a function is meant only for internal use.
- A single trailing underscore, such as with `max_`, is used by convention when you want to avoid a conflict with existing Python names or keywords.
- The **LEGB** Rule for Searching Names in Python:
  > You’re referencing x from inside an inner function. In this situation, Python looks for x in the following order:
  > - **Local**: Python searches for x inside the inner function. If it doesn’t find x there, then it moves to the enclosing scope.
  > - **Enclosing**: Next, Python searches for x in the enclosing function’s scope. If it’s not found there, then it moves to the global scope.
  > - **Global**: Python searches for x in the global scope. If it still doesn’t find it, it moves to the built-in scope.
  > - **Built-in**: Finally, Python searches for x in the built-in scope. If it doesn’t find x there, then it raises a `NameError` exception.
- getters and setters in Class
- use only `PascalCase` for classess (no `camelCase` or `snake_case`)
- You **shouldn’t use classes** when you need to:
  > - **Storing only data**. Use a data class, enumeration, or a named tuple instead. Data classes, enumerations, and named tuples are specially designed to store data. So, they might be the best solution if your class doesn’t have any behavior attached.
  > - **Providing a single method**. Use a function instead. If your class has a single method in its API, then you may not require a class. Instead, use a function unless you need to retain a certain state between calls. If more methods appear later, then you can always create a class.
  > - Avoid creating **custom classes to wrap up functionality** that’s available through built-in types or third-party classes. Use the type or third-party class directly.
  > - **A performance-critical program**. Classes add overhead to your program, especially when you need to create many objects. This may affect your code’s general performance.
- `__slots__` is a special feature in Python classes. By default, every object stores its attributes in `__dict__`. This makes attribute access flexible, but it also adds memory overhead. If you add `__slots__` to your class, you tell Python exactly which attributes are allowed. Python then skips creating a `__dict__` for each object, which saves memory and speeds up attribute access.
- In the standard `functools` library, a Least Recently Used (LRU) cache is available as `@functools.lru_cache`. Additionally, you can use a regular cache with `@functools.cache`.
- 
