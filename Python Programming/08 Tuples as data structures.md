## Tuples in Python: A foundational data structure for organizing data

In Python, a **Tuple** is one of the most fundamental ways to store a collection of values in a single variable. Think of it as a container that can hold multiple items together in one place. Tuples are particularly useful when you want to group related pieces of information, especially when that information should not change once it is defined.

Let’s begin with a few simple examples.

### 🧪 Defining Tuples in Python

Here’s how you can create a Tuple:

```python
# Tuple with multiple items
person = ("Alice", 28, "Engineer")
print(person)
```

**Output:**

```
('Alice', 28, 'Engineer')
```

You can even create a Tuple with just one item, but you must remember to include a comma — otherwise, Python will not treat it as a Tuple.

```python
# Tuple with a single item (notice the comma!)
single_item = ("Python",)
print(single_item)
```

**Output:**

```
('Python',)
```

If the comma is omitted, Python will treat it as a plain string:

```python
not_a_tuple = ("Python")
print(not_a_tuple)
```

**Output:**

```
Python
```

---

## Key Properties of Tuples

Let’s now understand what makes Tuples unique and why they exist alongside other data structures in Python.

### ✅ Tuples Can Store Heterogeneous Data

Tuples can store different types of data together — strings, numbers, even other collections — all in one container.

```python
car_details = ("Tesla", 2024, 79999.99, True)
print(car_details)
```

**Output:**

```
('Tesla', 2024, 79999.99, True)
```

This makes Tuples ideal when you’re trying to capture a single record or entity with multiple attributes.

---

### 📏 No Limit to the Number of Items

There’s no fixed size. A Tuple can hold just one item or hundreds of them — depending on what your program needs.

```python
coordinates = (45.123, 67.890, 12.456, 33.333)
print(coordinates)
```

---

### 🔢 Tuples Remember the Order of Items

Tuples maintain the order in which you added the items. This order is preserved, and each item can be accessed using its position — known as its **index**.

* Indexing starts from `0` for the first item
* Python also allows **negative indexing**, where `-1` refers to the last item, `-2` to the second last, and so on

```python
colors = ("Red", "Green", "Blue", "Yellow")

# Accessing by positive index
print(colors[0])    # First item
print(colors[2])    # Third item

# Accessing by negative index
print(colors[-1])   # Last item
print(colors[-3])   # Third item from end
```

**Output:**

```
Red
Blue
Yellow
Green
```

---

### 🔒 Tuples Are Immutable: You Can’t Change Them

Once a Tuple has been created, its items cannot be modified. This means:

* You can’t add new items
* You can’t remove existing items
* You can’t change the value of any item

This might sound restrictive at first, but there’s a strong reason behind it.

Imagine you’ve issued a fee receipt to a student or generated a timestamped record in a data logging system. Once this record is created, you wouldn’t want anyone to accidentally change it. That’s exactly the kind of situation where Tuples shine.

Here’s a relatable everyday example:

```python
birth_record = ("John", "15-Mar-2010", "City Hospital")
# Trying to change the name
birth_record[0] = "Johnny"  # ❌ This will raise an error
```

**Output:**

```
TypeError: 'tuple' object does not support item assignment
```

In the world of data science, Tuples are often used to store reference values or fixed configurations — anything that should not change once defined.

---

## Accessing Items from a Tuple

Knowing how to access individual items from a Tuple is important because you’ll often need to use or process a specific value.

You’ve already seen this with **indexing**, where you directly specify the position of the item.

But what if you want to access a group of items? That’s where **slicing** comes in.

### ✂️ Slicing Tuples

Slicing lets you extract a portion of the Tuple — a few items at a time — using a simple notation.

```python
days = ("Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun")
```

#### 👉 Left to Right Slicing

```python
print(days[1:4])  # Items from index 1 to 3 (4 is not included)
```

**Output:**

```
('Tue', 'Wed', 'Thu')
```

#### 👉 Right to Left Slicing (with negative indexes)

```python
print(days[-4:-1])  # 4th last to 2nd last
```

**Output:**

```
('Thu', 'Fri', 'Sat')
```

#### 👉 Slicing Without Providing Start or End

```python
# From start to index 3
print(days[:4])

# From index 3 to end
print(days[3:])

# The entire Tuple
print(days[:])
```

**Output:**

```
('Mon', 'Tue', 'Wed', 'Thu')
('Thu', 'Fri', 'Sat', 'Sun')
('Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun')
```

### 🧠 Why Slicing Is Useful

Let’s say you want to display only weekdays from the full list of days, or maybe just the weekend. Slicing helps you select only the part of the data that’s relevant for the task — without having to create a new structure from scratch.

---

## ✅ Summary

* Tuples help store multiple values in one variable
* They are great for keeping information that should not change
* Each item has a position (index), so you can pick out what you need
* You can also take a portion of the Tuple using slicing

As we move forward, you’ll see just how useful Tuples are — not just as a beginner-level data structure, but as a reliable tool used by professionals across real-world applications.
