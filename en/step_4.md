<h2 class="c-project-heading--task">A random password</h2>

--- task ---
Improve your program to create a longer password by adding random characters one at a time.
--- /task ---

--- task ---
To start with, your `password` variable should be empty.

Add this line to your code.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 5
---
import random

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'

password = ''
password = random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
You want to choose a random character 10 times.

To do this, add the following line.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 6
---
import random

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'

password = ''
for c in range(10):
password = random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
Indent the line that chooses a random character so that it happens 10 times.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 7
---
import random

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'

password = ''
for c in range(10):
    password = random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
Use `+=` to add the new character to the password each time.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 7
---
import random

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'

password = ''
for c in range(10):
    password += random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
**Test:** Click the **Run** button.

You should see a password that is 10 characters long.
--- /task ---

--- task ---
Try changing the number `10` to a bigger number and run your code again to see the results.
--- /task ---
