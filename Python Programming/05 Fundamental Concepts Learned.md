
# Core programming concepts behind the examples

In the previous section, you wrote simple programs and practiced solving a few problems. Now, let's slow down a little and understand the **core programming concepts** behind those examples — this will help you write your own programs much more easily!

We'll use the same familiar examples you have already seen, so it will feel natural.

---

# 1. Variables and Values

Remember the example where we calculated the **Area of a Rectangle**?  
Let's bring it back here for a moment:

```python
length = 10
width = 6
area = length * width
print("The area of the rectangle is:", area)
```

Now, let's slow down and break this down carefully.  
While we do that, you'll start picking up the **core ideas of Python programming** — and trust me, this will make everything else a lot easier later!

---

## 1.1 What is a Variable? What is a Value?

In Python, a **variable** is simply a name you give to a piece of information.  
The **value** is the actual data you are storing.

In our example:

- `length` and `width` are **variables**.
- `10` and `6` are the **values** assigned to them.

You can think of it like labeling a box:

```
Variable name (length)  <--  holds --> Value (10)
Variable name (width)   <--  holds --> Value (6)
```

The variable name helps you **refer back to that value later** — without hardcoding it again and again!

---

## 1.2 Explanation of the Assignment operation with `=` operator

The `=` symbol is called the **assignment operator** in Python.

When you write:

```python
length = 10
```

It means:  
👉 Take the value `10` and assign it to the name `length`.

Similarly:

```python
area = length * width
```

👉 First **calculate** `length * width` (which is `10 * 6 = 60`),  
👉 then **assign** that result `60` to the variable `area`.

In Python, **the right-hand side (RHS) is always evaluated first**, and the result is assigned to the left-hand side (LHS) variable.

---

## 1.3 Some Important Points about Assignment

### 1.3.1 No need to define variable types beforehand

Unlike some other languages, in Python you don't have to say "this will be an integer" or "this will be text".

You just assign a value and Python understands!

Example:

```python
age = 25            # Python understands this is an integer
name = "Charlie"    # Python understands this is text (string)
temperature = 37.5  # Python understands this is a decimal (float)
```

This makes writing code faster and easier — you just focus on **what** you want to store, not **how** to store it.

---

### 1.3.2 Longer expressions on the RHS

As programs grow, you'll see slightly more complex calculations on the right-hand side.

Example:

```python
average_speed = (distance1 + distance2 + distance3) / (time1 + time2 + time3)
```

Tip:  
Whenever you see a longer RHS, **mentally break it down into steps**:

- First add up all distances.
- Then add up all times.
- Then divide.

**Always remember:**  
👉 **RHS gets calculated first** → **then assigned to the LHS variable**.

---

### 1.3.3 Variables can update themselves

This is an important idea, and it will appear very often later.

Look at this:

```python
score = 80
score = score + 5
print(score)
```

Here’s what happens:

- First, `score` is assigned the value `80`.
- Then, `score = score + 5` means:
  - Take the **current value of `score`** (which is 80),
  - **Add 5** to it (80 + 5 = 85),
  - **Store** the new value `85` back into `score`.

After that, when you print `score`, it shows `85`.

> 📌 Think of it like **updating a box**:  
> You first had a box labeled `score` holding 80.  
> You opened the box, added 5 more, and closed it back with the new total 85 inside.

This kind of updating helps programs track things like totals, scores, balances, etc. dynamically.

---

## 1.4 Why are Variables so Important?

Imagine if you had to **hardcode** every single number directly inside every formula!  
It would become a mess very quickly — and making changes would be super painful.

Variables make programs:

- **Dynamic**: If a value changes (say, the `length`), your program adjusts automatically.
- **Easier to update**: You only change the value in one place — no manual hunting through code.
- **Less error-prone**: Fewer chances of making a mistake by manually updating numbers everywhere.

In short:  
👉 Variables make your programs **flexible**, **clean**, and **smart**.

---

# 2. Operators in Python

In the earlier examples, you saw that we were using symbols like `+`, `-`, `*`, `/` to perform simple calculations.  
These are called **operators**.

Operators allow you to perform operations on values or variables. In Python, there are **different types of operators** depending on what kind of operation you want to perform.

Let's explore them one by one!

---

## 2.1 Arithmetic Operators

These are the operators that help you perform basic math operations.

Here’s a quick overview:

| Operator | Meaning                      | Example            | Result |
|:--------:|:------------------------------|:------------------:|:------:|
| `+`      | Addition                      | `5 + 3`             | `8`    |
| `-`      | Subtraction                   | `5 - 3`             | `2`    |
| `*`      | Multiplication                 | `5 * 3`             | `15`   |
| `/`      | Division (float result)        | `5 / 2`             | `2.5`  |
| `//`     | Floor Division (quotient only)  | `5 // 2`            | `2`    |
| `%`      | Modulo (remainder)              | `5 % 2`             | `1`    |
| `**`     | Exponent (power)                | `2 ** 3`            | `8`    |

> ✨ **Note:**  
> - `/` always gives a decimal result.  
> - `//` gives only the whole number part, dropping the decimal part.  
> - `%` gives the remainder left after division.

---

## 2.2 Comparison Operators

These operators are used when you want to **compare** two values.

They always give you a result of either **True** or **False** (this is super important for conditions later on).

Here’s the table:

| Operator | Meaning                        | Example          | Result  |
|:--------:|:-------------------------------|:----------------:|:-------:|
| `==`     | Equal to                        | `5 == 5`         | `True`  |
| `!=`     | Not equal to                    | `5 != 3`         | `True`  |
| `>`      | Greater than                    | `5 > 3`          | `True`  |
| `<`      | Less than                       | `5 < 3`          | `False` |
| `>=`     | Greater than or equal to         | `5 >= 5`         | `True`  |
| `<=`     | Less than or equal to            | `5 <= 6`         | `True`  |

> ✨ **Note:**  
> - `=` (single equal) is for assignment.  
> - `==` (double equal) is for checking equality, i.e. if the Left hand side (LHS) is exactly equal to the Right hand side (RHS)

---

## 2.3 A Quick Reality Check

Let’s say you are writing a program to calculate someone's final marks and check if they have passed.

You could use arithmetic operators to calculate total marks, and comparison operators to check if the marks are more than the pass mark!

Example:

```python
total_marks = 400
pass_marks = 350

# Check if passed
has_passed = total_marks >= pass_marks
print(has_passed)    # Output: True
```

---

## 2.4 Operator Precedence (Order of Operations)

When you have a bigger expression with many operators, Python **follows an order** to decide **which operation happens first**.

The basic rules (same as math):

1. **Parentheses** `()` → Always done first
2. **Exponents** `**`
3. **Multiplication `*`, Division `/`, Floor Division `//`, Modulo `%`** → Left to right
4. **Addition `+` and Subtraction `-`** → Left to right
5. **Comparisons** (`==`, `!=`, `>`, `<`, etc.) happen after the arithmetic is fully evaluated.

---

### Example:

```python
result = 5 + 3 * 2 ** 2 - (8 // 3)
print(result)
```

Let's break it down:

- First, exponent: `2 ** 2 = 4`
- Then, multiplication: `3 * 4 = 12`
- Then, floor division inside parentheses: `8 // 3 = 2`
- Now substitute back: `5 + 12 - 2`
- Addition: `5 + 12 = 17`
- Subtraction: `17 - 2 = 15`

Final output:

```
15
```

> 📌 **Tip:**  
> Whenever you are unsure about order, use parentheses `()` to control it yourself!

---

## 3. Functions – Understanding `print()`

A **function** is like a mini-program built into Python, ready to perform a specific task when you call it.

The first function you are using is `print()` — it **displays information on the screen**.

Example:
```python
print("The perimeter is:", perimeter, "units")
```

Inside `print()`:
- Strings like `"The perimeter is:"` are shown exactly as they are.
- Variables like `perimeter` show their current value.
- Commas `,` are used to separate multiple items — Python adds spaces automatically between them.

---

### Some important points about functions:
- **Functions always use round brackets `()`** in Python.
- **Functions are built for a specific purpose** — like printing, adding numbers, checking conditions, etc.
- **Many built-in functions exist** in Python.  
  Some examples are:
  - `print()` — display something
  - `len()` — find the length of something (like how many letters in a word)
  - `type()` — check what type of value (number, text, etc.)

**Example**:
```python
name = "Alex"
print(len(name))    # Shows: 4
```

As you move forward, you will learn how to use many more functions, and even how to **create your own functions**!

---

# Summary

In every program you wrote earlier, three powerful ideas were working together:
- **Variables**: to store values,
- **Operators**: to perform calculations,
- **Functions**: to carry out specific actions (like printing results).

The better you understand these basics, the easier and more fun programming becomes!

---

✅ **Next Steps**:
- Try defining your own variables and performing calculations.
- Play with different operators.
- Explore using more functions like `len()` and `type()`.

---
