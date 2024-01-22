In this project, I acquired skills in managing Python errors and exceptions using the `try` and `except` blocks.

## Function Prototypes :floppy_disk:

This section lists the prototypes of functions developed in this project:

| File                             | Prototype                                               |
| -------------------------------- | ------------------------------------------------------- |
| `0-safe_print_list.py`           | `def safe_print_list(my_list=[], x=0):`                 |
| `1-safe_print_integer.py`        | `def safe_print_integer(value):`                        |
| `2-safe_print_list_integers.py`  | `def safe_print_list_integers(my_list=[], x=0):`        |
| `3-safe_print_division.py`       | `def safe_print_division(a, b):`                        |
| `4-list_division.py`             | `def list_division(my_list_1, my_list_2, list_length):` |
| `5-raise_exception.py`           | `def raise_exception():`                                |
| `6-raise_exception_msg.py`       | `def raise_exception_msg(message=""):`                  |
| `100-safe_print_integer_err.py`  | `def safe_print_integer_err(value):`                    |
| `101-safe_function.py`           | `def safe_function(fct, *args):`                        |
| `102-magic_calculation.py`       | `def magic_calculation(a, b);`                          |
| `103-python.c`                   | <ul><li>`void print_python_list(PyObject *p);`</li><li>`void print_python_bytes(PyObject *p);`</li><li>`void print_python_float(PyObject *p);`</li></ul> |

## Tasks :page_with_curl:

* **0. Safe list printing**
  * [0-safe_print_list.py](./0-safe_print_list.py): A Python function that prints up to `x` elements of a list on the same line, ending with a new line.
  * The parameter `x` signifies the number of elements to print and may exceed the list's length.
  * It returns the actual count of elements printed.
  * No module imports or `len()` usage.

* **1. Safe printing of an integers list**
  * [1-safe_print_integer.py](./1-safe_print_integer.py): A Python function that prints an integer using the `"{:d}".format()` format.
  * The `value` parameter can be of any type.
  * It returns `True` if `value` was an integer and printed correctly, `False` otherwise.
  * No module imports or `type()` usage.

* **2. Print and count integers**
  * [2-safe_print_list_integers.py](./2-safe_print_list_integers.py): A Python function that prints the first `x` elements of a list that are integers, followed by a new line.
  * The `my_list` parameter may contain any type.
  * The `x` parameter signifies the number of elements to print and may be larger than the list's length.
  * It returns the actual count of integers printed.
  * No module imports or `len()` usage.

* **3. Integers division with debug**
  * [3-safe_print_division.py](./3-safe_print_division.py): A Python function that divides two integers and prints the result using `finally:`.
  * Assumes the arguments are integers.
  * Returns the division value upon success; `None` otherwise.
  * No module imports.

* **4. Divide a list**
  * [4-list_division.py](./4-list_division.py): A Python function that divides two lists element-wise.
  * Creates a new list of length `list_length` with the results of the divisions.
  * Both `my_list_1` and `my_list_2` can contain any type.
  * The `list_length` parameter may exceed either list's length.
  * If an element is not a number, prints `wrong type`.
  * Prints `division by 0` if a division cannot be done and `out of range` if a list is too short.
  * No module imports.

* **5. Raise exception**
  * [5-raise_exception.py](./5-raise_exception.py): A Python function that triggers a type exception.
  * No module imports.

* **6. Raise a message**
  * [6-raise_exception_msg.py](./6-raise_exception_msg.py): A Python function that raises a name exception with a message.
  * No module imports.

* **7. Safe integer print with error message**
  * [100-safe_print_integer_err.py](./100-safe_print_integer_err.py): A Python function that prints an integer with type-checking in the `"{:d}".format()` format.
  * The `value` parameter can be any type.
  * Returns `True` if `value` is an integer and

 was printed correctly.
  * If not, it prints an exception error to `stderr` and returns `False`.
  * No module imports.

* **8. Safe function**
  * [101-safe_function.py](./101-safe_function.py): A Python function that safely executes another function.
  * Assumes `fct` is always a function pointer.
  * Returns the function's result upon success; `None` otherwise.
  * Prints an exception error to `stderr` if there's an error.

* **9. ByteCode -> Python #4**
  * [102-magic_calculation.py](./102-magic_calculation.py): A Python function that exactly matches a given bytecode from ALX-Africa.

* **10. CPython #2: PyFloatObject**
  * [103-python.c](./103-python.c): C functions that display basic information about Python list, byte, and float objects.