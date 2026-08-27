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

