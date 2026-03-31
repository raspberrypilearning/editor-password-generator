<h2 class="c-project-heading--task">Random characters</h2>

### Step 1
Create a program that generates and prints a single random character.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 3-6
---
import random                     # Import tools for choosing random items

chars = 'abcdefghijklmnopqrstuvwxyz1234567890'  # A string of characters the password can use (letters and numbers)

password = random.choice(chars)   # Pick one random character from chars
print(password)                   # Show the password on the screen

--- /code ---
</div>

### Step 2
**Test:** Click **Run**.

You should see a single character printed on the screen.  
Run the program several times — the character should change, and sometimes it should be a number.
