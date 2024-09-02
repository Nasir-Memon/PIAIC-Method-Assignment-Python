In Python, "methods" refer to functions that are associated with an object. Methods are similar to functions, but they are called on an object and have access to the object’s attributes. Here are some common Python methods along with examples:

### 1. **String Methods**
- **`str.upper()`**: Converts all characters of a string to uppercase.
    ```python
    text = "hello"
    print(text.upper())  # Output: "HELLO"
    ```
- **`str.lower()`**: Converts all characters of a string to lowercase.
    ```python
    text = "HELLO"
    print(text.lower())  # Output: "hello"
    ```
- **`str.strip()`**: Removes any leading and trailing whitespace.
    ```python
    text = "   hello   "
    print(text.strip())  # Output: "hello"
    ```
- **`str.replace(old, new)`**: Replaces all occurrences of a substring with another substring.
    ```python
    text = "hello world"
    print(text.replace("world", "Python"))  # Output: "hello Python"
    ```
- **`str.split(separator)`**: Splits a string into a list where each word is a list item.
    ```python
    text = "hello world"
    print(text.split())  # Output: ['hello', 'world']
    ```

### 2. **List Methods**
- **`list.append(item)`**: Adds an item to the end of the list.
    ```python
    fruits = ["apple", "banana"]
    fruits.append("cherry")
    print(fruits)  # Output: ['apple', 'banana', 'cherry']
    ```
- **`list.remove(item)`**: Removes the first occurrence of an item from the list.
    ```python
    fruits = ["apple", "banana", "cherry"]
    fruits.remove("banana")
    print(fruits)  # Output: ['apple', 'cherry']
    ```
- **`list.pop(index)`**: Removes and returns the item at the given index. If no index is specified, it removes the last item.
    ```python
    fruits = ["apple", "banana", "cherry"]
    popped_item = fruits.pop()
    print(popped_item)  # Output: "cherry"
    print(fruits)  # Output: ['apple', 'banana']
    ```
- **`list.sort()`**: Sorts the items in ascending order.
    ```python
    numbers = [3, 1, 4, 1, 5]
    numbers.sort()
    print(numbers)  # Output: [1, 1, 3, 4, 5]
    ```
- **`list.reverse()`**: Reverses the order of the list items.
    ```python
    numbers = [3, 1, 4, 1, 5]
    numbers.reverse()
    print(numbers)  # Output: [5, 1, 4, 1, 3]
    ```

### 3. **Dictionary Methods**
- **`dict.get(key, default=None)`**: Returns the value for the specified key if the key is in the dictionary, otherwise returns the default value.
    ```python
    person = {"name": "Alice", "age": 25}
    print(person.get("name"))  # Output: "Alice"
    print(person.get("gender", "Not specified"))  # Output: "Not specified"
    ```
- **`dict.keys()`**: Returns a view object that displays a list of all the keys in the dictionary.
    ```python
    person = {"name": "Alice", "age": 25}
    print(person.keys())  # Output: dict_keys(['name', 'age'])
    ```
- **`dict.values()`**: Returns a view object that displays a list of all the values in the dictionary.
    ```python
    person = {"name": "Alice", "age": 25}
    print(person.values())  # Output: dict_values(['Alice', 25])
    ```
- **`dict.items()`**: Returns a view object that displays a list of dictionary's key-value tuple pairs.
    ```python
    person = {"name": "Alice", "age": 25}
    print(person.items())  # Output: dict_items([('name', 'Alice'), ('age', 25)])
    ```
- **`dict.update(other_dict)`**: Updates the dictionary with elements from another dictionary object or from an iterable of key-value pairs.
    ```python
    person = {"name": "Alice", "age": 25}
    update = {"age": 26, "city": "New York"}
    person.update(update)
    print(person)  # Output: {"name": "Alice", "age": 26, "city": "New York"}
    ```

### 4. **Set Methods**
- **`set.add(item)`**: Adds an item to the set.
    ```python
    fruits = {"apple", "banana"}
    fruits.add("cherry")
    print(fruits)  # Output: {'apple', 'banana', 'cherry'}
    ```
- **`set.remove(item)`**: Removes an item from the set. If the item is not found, it raises a KeyError.
    ```python
    fruits = {"apple", "banana", "cherry"}
    fruits.remove("banana")
    print(fruits)  # Output: {'apple', 'cherry'}
    ```
- **`set.union(other_set)`**: Returns a new set with all items from both sets.
    ```python
    set1 = {"apple", "banana"}
    set2 = {"cherry", "banana"}
    print(set1.union(set2))  # Output: {'apple', 'banana', 'cherry'}
    ```
- **`set.intersection(other_set)`**: Returns a new set containing only items that exist in both sets.
    ```python
    set1 = {"apple", "banana"}
    set2 = {"banana", "cherry"}
    print(set1.intersection(set2))  # Output: {'banana'}
    ```
- **`set.difference(other_set)`**: Returns a new set with items that are only in the first set and not in the second.
    ```python
    set1 = {"apple", "banana"}
    set2 = {"banana", "cherry"}
    print(set1.difference(set2))  # Output: {'apple'}
    ```

### 5. **File Methods**
- **`file.read(size=-1)`**: Reads the file’s content, if `size` is specified, it reads up to that many bytes/characters.
    ```python
    with open("example.txt", "r") as file:
        content = file.read()
        print(content)
    ```
- **`file.write(text)`**: Writes the specified text to the file.
    ```python
    with open("example.txt", "w") as file:
        file.write("Hello, World!")
    ```
- **`file.readlines()`**: Reads all lines in a file and returns them as a list.
    ```python
    with open("example.txt", "r") as file:
        lines = file.readlines()
        print(lines)
    ```
- **`file.close()`**: Closes the opened file. (Using `with` statements automatically closes the file.)
    ```python
    file = open("example.txt", "r")
    content = file.read()
    file.close()
    ```
  
These are some of the commonly used methods in Python, each associated with different data types such as strings, lists, dictionaries, sets, and files. Each method serves a specific purpose and helps in manipulating and working with the corresponding data type.