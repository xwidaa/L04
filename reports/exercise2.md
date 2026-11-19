# Bug reports for exercise2.py

Line: 3
Problem: The condition checks if the grade is greater than 5, but the docstring says "True if the grade is 5 or more", which means it should include 5. The correct condition is >= instead of >.
Example: input: 5, actual output: False, expected output: True
Fix: return grade >= 5

Line: 8
Problem: The function checks if the password has at least one digit using any(c.isdigit() for c in password), but it does not verify that the password has at least 8 characters. The condition is reversed: it uses len(password) > 8 instead of >= 8.
Example: input: "pass1234", actual output: False, expected output: True
Fix: return len(password) >= 8 and any(c.isdigit() for c in password)

Line: 12
Problem: The clamp function incorrectly uses min(x, low) and then max(low, min(x, low)), which results in always returning low. It should return max(low, min(x, high)) to properly clamp between low and high.
Example: input: x=3, low=1, high=10, actual output: 1, expected output: 3
Fix: return max(low, min(x, high))
