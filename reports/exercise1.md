# Bug reports for exercise1.py

Line: 3
Problem: The condition `n % 2 == 1` checks if a number is odd, not even. For even numbers, the remainder when divided by 2 should be 0, not 1. This is the opposite of what the function is supposed to do.
Example: is_even(4) returns False (actual), but should return True (expected)
Fix: return n % 2 == 0

Line: 8
Problem: The function calculates the sum of width and height, not the area of a rectangle. The area of a rectangle is width multiplied by height, not added.
Example: rectangle_area(5, 3) returns 8 (actual), but should return 15 (expected)
Fix: return width * height

Line: 13
Problem: The function adds 2 to n instead of doubling it. "Twice the number n" means multiplying by 2, not adding 2.
Example: double(3) returns 5 (actual), but should return 6 (expected)
Fix: return n * 2
