# Labs 1–5: Getting Started with Python

> A detailed, beginner-friendly walkthrough of the first five labs from the roadmap.
> Each lab has: **Concept** (what & why) → **Example** (worked code) → **Lab Practice** (you do it) → **Solution**.
>
> Work through these in order. Type every example yourself — do not copy-paste. Typing builds muscle memory.

---

## Table of Contents
1. [Lab 1 — Install Python & Verify](#lab-1--install-python--verify)
2. [Lab 2 — The REPL](#lab-2--the-repl)
3. [Lab 3 — Running a Script](#lab-3--running-a-script)
4. [Lab 4 — Comments & Docstrings](#lab-4--comments--docstrings)
5. [Lab 5 — Variables & Assignment](#lab-5--variables--assignment)

---

## Lab 1 — Install Python & Verify

### Concept
Python is a **programming language**, and to run Python code your computer needs the **Python interpreter** — a program that reads your code and executes it line by line.

Two important ideas:
- **Interpreter**: The software (`python.exe` on Windows) that runs your `.py` files. When you "install Python," you are installing this interpreter plus its standard library.
- **PATH**: An environment variable that tells your operating system *where* to find programs. If Python is "on the PATH," you can type `python` from any folder and the OS knows where to find it. If it is not on the PATH, the terminal says "python is not recognized."

Why version matters: Python 3.12+ has modern features and better error messages. Python 2 is dead — never use it. Always confirm your version so you know what features are available.

### Example
After installing Python from [python.org](https://www.python.org/downloads/) (check the box **"Add Python to PATH"** during install), open a **new** PowerShell window and run:

```powershell
python --version
```

Expected output (your exact number may differ):

```text
Python 3.12.4
```

You can also list every Python version installed on Windows using the **py launcher**:

```powershell
py -0p
```

Example output:

```text
 -V:3.12 *        C:\Users\Dell\AppData\Local\Programs\Python\Python312\python.exe
 -V:3.11          C:\Users\Dell\AppData\Local\Programs\Python\Python311\python.exe
```

The `*` marks the default version. The path on the right is *where* the interpreter lives.

### Lab Practice
1. Install Python 3.12 or newer (remember to check "Add Python to PATH").
2. Open a **new** terminal and confirm the version with `python --version`.
3. List all installed versions with `py -0p`.
4. Find out where your default Python lives by running `where python` (Windows).

### Solution
```powershell
python --version        # -> Python 3.12.x
py -0p                   # -> lists all installed versions, * = default
where python             # -> C:\Users\...\Python312\python.exe
```
If `python --version` fails with "not recognized," Python is not on your PATH. Fix it by re-running the installer and checking **"Add Python to PATH"**, or add the folder shown by `py -0p` to your PATH manually.

---

## Lab 2 — The REPL

### Concept
**REPL** stands for **Read–Eval–Print Loop**:
- **Read**: it reads the line you type,
- **Eval**: it evaluates (runs) it,
- **Print**: it prints the result,
- **Loop**: it waits for your next line.

The REPL is an **interactive shell** — a scratchpad where you can test tiny pieces of code instantly without creating a file. It is perfect for experiments: "What does this function return? What type is this value?" You'll use it constantly while learning.

Key detail: In the REPL, typing an expression like `2 + 2` **automatically shows** the result. In a script file, you would need `print(2 + 2)` to see it. This difference confuses beginners, so remember it.

### Example
Start the REPL by typing `python` (no filename) and pressing Enter:

```powershell
python
```

You'll see the `>>>` prompt. Now type expressions:

```python
>>> 2 + 2
4
>>> 10 * 5
50
>>> print("hi")
hi
>>> name = "AI"
>>> name
'AI'
>>> name.upper()
'AI'
```

Notice:
- `2 + 2` showed `4` automatically (it's an expression).
- `print("hi")` showed `hi` without quotes (print displays text).
- `name` (just typing the variable) showed `'AI'` **with** quotes — that's the REPL showing you the raw value (a string).

Exit the REPL with:

```python
>>> exit()
```

(or press `Ctrl+Z` then Enter on Windows).

### Lab Practice
1. Open the REPL.
2. Calculate `2 + 2`.
3. Print the text `Hello AI` using `print()`.
4. Compute how many seconds are in a day (`24 * 60 * 60`).
5. Exit the REPL cleanly.

### Solution
```python
>>> 2 + 2
4
>>> print("Hello AI")
Hello AI
>>> 24 * 60 * 60
86400
>>> exit()
```

---

## Lab 3 — Running a Script

### Concept
The REPL is great for quick tests, but real programs live in **script files** — plain text files ending in `.py`. A script is a saved list of instructions the interpreter runs top to bottom, all at once.

Two ways to run Python, and when to use each:

| | REPL | Script (`.py` file) |
|---|---|---|
| **How** | type `python`, then code line by line | write code in a file, run `python file.py` |
| **Best for** | quick experiments, testing one idea | real programs you save, reuse, and share |
| **Output** | expressions auto-print | must use `print()` to see anything |
| **Persistence** | lost when you close it | saved to disk forever |

Critical rule for scripts: **nothing prints unless you call `print()`.** Writing `2 + 2` on its own line in a script computes the result and then throws it away silently.

### Example
Create a file named `hello.py` with this content:

```python
print("Hello AI")
```

Then run it from the terminal (make sure you're in the same folder as the file):

```powershell
python hello.py
```

Output:

```text
Hello AI
```

Now try a script with **multiple lines** to see top-to-bottom execution. Create `math_demo.py`:

```python
print("Starting calculations...")
result = 24 * 60 * 60
print("Seconds in a day:", result)
print("Done!")
```

Run it:

```powershell
python math_demo.py
```

Output:

```text
Starting calculations...
Seconds in a day: 86400
Done!
```

Notice the lines ran **in order**, and only the `print()` lines produced visible output — the `result = ...` line ran silently.

### Lab Practice
1. Create a file `hello.py` that prints `Hello AI`.
2. Run it with `python hello.py`.
3. Create a second file `about_me.py` that prints your name, then your favorite topic, on two separate lines.
4. Add a line that computes `100 * 7` — but **without** `print()`. Run it and notice nothing shows for that line.
5. Wrap that calculation in `print()` and run again to see the result.

### Solution
`hello.py`:
```python
print("Hello AI")
```

`about_me.py`:
```python
print("My name is Dell")
print("My favorite topic is Artificial Intelligence")

100 * 7            # runs but shows nothing — the result is discarded
print(100 * 7)     # now it shows: 700
```

Run:
```powershell
python hello.py
python about_me.py
```

---

## Lab 4 — Comments & Docstrings

### Concept
As programs grow, you (and others) need to understand *why* code does what it does. Python gives you two documentation tools:

**1. Comments** — Notes for humans that the interpreter completely ignores. They start with `#`. Everything after `#` on that line is skipped when the code runs. Use them to explain *why*, not *what* (good code already shows *what*).

```python
# This is a comment. Python ignores it.
x = 5  # An inline comment: explains this specific line.
```

**2. Docstrings** — A special string (wrapped in triple quotes `"""..."""`) placed at the very top of a file, function, or class. Unlike comments, docstrings are **stored by Python** and can be read at runtime (e.g., by help tools and IDEs). They describe *what a piece of code does* as official documentation.

```python
"""This module greets the user."""
```

Difference in one line: a **comment** is an ignored side-note; a **docstring** is retrievable documentation attached to code.

### Example
Create `greet.py`:

```python
"""greet.py — A tiny program that greets an AI learner.

This top-of-file docstring explains the file's purpose.
Tools like help() and VS Code can read it.
"""

# Define the message we want to show.
message = "Hello AI learner"   # inline comment: our greeting text

# Print the greeting to the screen.
print(message)
```

Run it:

```powershell
python greet.py
```

Output:

```text
Hello AI learner
```

The docstring and comments produced **no output** — they exist only to explain the code. But the docstring *is* retrievable. Prove it in the REPL:

```python
>>> import greet
Hello AI learner
>>> print(greet.__doc__)
greet.py — A tiny program that greets an AI learner.

This top-of-file docstring explains the file's purpose.
Tools like help() and VS Code can read it.
```

The comments are gone (ignored), but `greet.__doc__` still holds the docstring. That's the key difference.

### Lab Practice
1. Add a top-of-file docstring to your `hello.py` from Lab 3 describing what it does.
2. Add at least one full-line comment and one inline comment.
3. Run the script and confirm the output is unchanged (comments/docstrings don't affect output).
4. In the REPL, import your module and print its `__doc__` to see the docstring.

### Solution
`hello.py`:
```python
"""hello.py — Prints a friendly greeting for AI learners."""

# Print the greeting message to the terminal.
print("Hello AI")   # this line does the actual work
```

Verify the docstring is stored:
```python
>>> import hello
Hello AI
>>> print(hello.__doc__)
hello.py — Prints a friendly greeting for AI learners.
```

---

## Lab 5 — Variables & Assignment

### Concept
A **variable** is a name that refers to a value stored in memory. **Assignment** uses the `=` sign to bind a name to a value:

```python
age = 25
```

Read this as: "the name `age` now refers to the value `25`." The `=` is **not** "equals" like in math — it means "assign the value on the right to the name on the left."

Two important Python properties:

**1. Dynamic typing** — You don't declare a variable's type. Python figures out the type from the value. The same name can even point to different types over time (though that's usually bad style):

```python
x = 5        # x refers to an integer
x = "hello"  # now x refers to a string — perfectly legal in Python
```

**2. Names are labels, not boxes** — A variable is a *label* pointing at a value in memory, not a container holding it. Reassigning just moves the label to a new value.

**Naming rules & conventions:**
- Must start with a letter or underscore; can contain letters, digits, underscores.
- Case-sensitive: `age` and `Age` are different.
- Use `snake_case` (lowercase with underscores): `first_name`, `total_score`.
- Choose descriptive names: `score` beats `s`.

**f-strings** are the modern way to insert variables into text. Put an `f` before the quote and wrap variables in `{}`:

```python
name = "AI"
print(f"Hello, {name}!")   # -> Hello, AI!
```

### Example
Create `variables.py`:

```python
"""variables.py — Demonstrates variables, assignment, and f-strings."""

# Assign different types of values to well-named variables.
name = "Dell"          # a string  (text)
age = 25               # an integer (whole number)
pi = 3.14159           # a float    (decimal number)
is_learning = True     # a boolean  (True/False)

# Use an f-string to build a sentence from the variables.
print(f"My name is {name} and I am {age} years old.")
print(f"The value of pi is roughly {pi}.")
print(f"Am I learning AI? {is_learning}")

# Reassigning: the label 'age' now points to a new value.
age = age + 1
print(f"Next year I will be {age}.")
```

Run it:

```powershell
python variables.py
```

Output:

```text
My name is Dell and I am 25 years old.
The value of pi is roughly 3.14159.
Am I learning AI? True
Next year I will be 26.
```

Check types in the REPL with the built-in `type()` function:

```python
>>> name = "Dell"
>>> age = 25
>>> pi = 3.14159
>>> type(name)
<class 'str'>
>>> type(age)
<class 'int'>
>>> type(pi)
<class 'float'>
```

### Lab Practice
1. Create three variables: `name` (your name, a string), `age` (a number), and `pi` (3.14159).
2. Print them in a single sentence using an f-string.
3. Add a fourth variable `favorite_topic` and include it in the sentence.
4. Reassign `age` to be one year older and print the new value.
5. In the REPL, use `type()` to confirm the type of each variable.

### Solution
`variables.py`:
```python
"""My first variables practice."""

name = "Dell"
age = 30
pi = 3.14159
favorite_topic = "Artificial Intelligence"

print(f"Hi, I'm {name}, I'm {age}, and I love {favorite_topic}. Pi is {pi}.")

age = age + 1
print(f"After my birthday I'll be {age}.")
```

Type checks:
```python
>>> type("Dell")   # <class 'str'>
>>> type(30)       # <class 'int'>
>>> type(3.14159)  # <class 'float'>
>>> type(True)     # <class 'bool'>
```

---

## Recap & What's Next

You just learned the absolute foundation:
- **Lab 1:** Installed the Python interpreter and verified it via the terminal.
- **Lab 2:** Used the REPL as an interactive scratchpad (auto-prints expressions).
- **Lab 3:** Wrote and ran `.py` script files (need `print()` to see output).
- **Lab 4:** Documented code with comments (ignored) and docstrings (retrievable).
- **Lab 5:** Created variables, understood dynamic typing, and formatted text with f-strings.

**Practice challenge (combines all 5):** Write a script `intro.py` with a docstring, a few comments, and variables for your name, age, and goal. Use an f-string to print a short introduction, then run it from the terminal.

**Next up:** Labs 6–10 cover numeric types, strings, string methods, f-string formatting, and booleans.
