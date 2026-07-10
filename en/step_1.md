## Random characters

Create a program that generates and prints a single random character.

```python filename="main.py" line_numbers="true" line_number_start="1" line_highlights="3-6"
import random                     # Import tools for choosing random items

chars = 'abcdefghijklmnopqrstuvwxyz1234567890'  # A string of characters the password can use (letters and numbers)

password = random.choice(chars)   # Pick one random character from chars
print(password)                   # Show the password on the screen

```

## Now run your code

Click on **Run**.

You should see a single character printed on the screen.

Run the program several times. The character should change, and sometimes it should be a number.
