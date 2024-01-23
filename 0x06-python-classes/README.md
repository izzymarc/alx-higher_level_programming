In this project, I delved into object-oriented programming by utilizing classes and objects in Python. My focus was on understanding and implementing attributes, methods, and properties, along with key concepts such as data abstraction, encapsulation, and information hiding.

## Tests :heavy_check_mark:

* [tests](./tests): This directory contains test files, courtesy of Holberton School.

## Tasks :page_with_curl:

* **0. My First Square**
  * [0-square.py](./0-square.py): This Python class, `Square`, represents a square.

* **1. Square with Size**
  * [1-square.py](./1-square.py): Enhances the `Square` class from [0-square.py](./0-square.py) by adding:
    * A private instance attribute `size`.
    * Initialization with `size`.

* **2. Size Validation**
  * [2-square.py](./2-square.py): Further develops the `Square` class from [1-square.py](./1-square.py) by:
    * Allowing initialization with an optional `size` (`def __init__(self, size=0):`).
    * Raising a `TypeError` for non-integer `size` values with the message `must be an integer`.
    * Raising a `ValueError` for `size < 0` with the message `size must be >= 0`.

* **3. Area of a Square**
  * [3-square.py](./3-square.py): Expands on [2-square.py](./2-square.py) by introducing:
    * A public instance method `def area(self):` that returns the current square area.

* **4. Access and Update Private Attribute**
  * [4-square.py](./4-square.py): Advances the `Square` class from [3-square.py](./3-square.py) by:
    * Adding a property `def size(self):` to retrieve `self`.
    * Including a property setter `def size(self, value):` to set `self`.

* **5. Printing a Square**
  * [5-square.py](./5-square.py): Builds upon [4-square.py](./4-square.py) by adding:
    * A public instance method `def my_print(self):` to print the square with `#`, or an empty line if `size` is 0.

* **6. Coordinates of a Square**
  * [6-square.py](./6-square.py): Continues from [5-square.py](./5-square.py) with:
    * A private instance attribute `position`.
    * A property `def position(self):` to retrieve `position`.
    * A property setter `def position(self, value):` to set `position`.
    * Initialization with optional `size` and `position`: `def __init__(self, size=0, position=(0, 0)):`
    * A `TypeError` for non-tuple `position` with the message `position must be a tuple of 2 positive integers`.

* **7. Singly Linked List**
  * [100-singly_linked_list.py](./100-singly_linked_list.py): Introduces Python classes `Node` and `SinglyLinkedList` for a singly-linked list. The `Node` class has:
    * A private instance attribute `data`.
    * A property `def data(self):` and a setter `def data(self, value):` for `data`.
    * A private instance attribute `next_node`.
    * A property `def next_node(self):` and a setter `def next_node(self, value):` for `next_node`.
    * Initialization with `data` and `next_node`: `def __init__(self, data, next_node=None):`
    * A `TypeError` for non-integer `data` with the message `data must be an integer`.
    * A `TypeError` for non-Node `next_node` with the message `next_node must be a Node object`.
  * The `SinglyLinkedList` class has:
    * A private instance attribute `head`.
    * An initializer `def __init__(self):`.
    * A public method `def sorted_insert(self, value):` for inserting a new `Node` in sorted order.

* **8. Print Square Instance**
  * [101-square.py](./101-square.py): Updates the `Square` class from [6-square.py](./6-square.py) by:
    * Implementing `__str__` method to make printing a `Square` instance equivalent to `my_print()`.

* **9. Compare 2 Squares**
  * [102-square.py](./102-square.py): Further refines the `Square` class from [101-square.py](./101-square.py) by adding:
    * Methods `__eq__`, `__ne__`, `__lt__`, `__le__`, `__gt__`, and `__ge__

`, for logical comparisons (`==`, `!=`, `<`, `<=`, `>`, `>=`) based on square area.

* **10. ByteCode -> Python #5**
  * [103-magic_class.py](./103-magic_class.py): A Python function precisely matching a provided bytecode.