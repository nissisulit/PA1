# PA1

**Name: SULIT, Nissi Aleichem B**. 

**Section: 2ECE-B**

**Date Submitted: August 27, 2026**

This Program Assignment has three different questions to be done. Performing each function for every task.

# **Problem 1: Word Rotation Problem**
In this problem, the goal is to rotate a word by taking its first character and placing it at the. For example, the word "python" would be changed to "npytho". To get this, there is a function called rotate_word() is created to rearrange the characters of the given word.

First, the program uses the input() function to ask the user for a word or text. The entered value is stored in the variable word, which is then passed to the rotate_word() function for processing. 

```python
def rotate_word(text):
    return text[1:] + text[0]

word = input("Enter text: ")
print(rotate_word(word))
```
# **Problem 2: Username Builder Problem**
For Problem 2, the objective is to create a function that generates a username using the user's first and last names. The resulting username must be written in lowercase, with a period (.) placed between the first and last names. For example, "Nissi" and "Sulit" would produce "nissi.sulit".

The program first asks the user to enter their first name using the input() function and stores the result in the variable first. It then requests the last name and saves it in the variable last. These two values are passed to the make_username() function, where spaces are removed and both names are converted to lowercase before being combined.


```python
def make_username(first_name, last_name):
    first_name = first_name.lower().replace(" ", "")
    last_name = last_name.lower().replace(" ", "")
    return first_name + "." + last_name

first = input("Enter first name: ")
last = input("Enter last name: ")
username = make_username(first, last)
print(username)
```
# **Problem 3: Bookend Swap Problem**
In Problem 3, the task is to create a function that exchanges the first and last elements of a list while keeping all the elements in between in their original positions. This process is referred to as a "bookend swap" because only the elements at both ends of the list are switched. For example, ["calculator", "multimeter", "paper"] would become ["paper", "multimeter", "calculator"].

```python
def swap_bookends(items):
    first, *middle, last = items
    return [last] + middle + [first]

items = input("Enter items: ")
initems = items.split()
swap = swap_bookends(initems)
print(swap)
```


