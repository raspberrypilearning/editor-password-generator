<h2 class="c-project-heading--task">Lots of passwords</h2>

--- task ---
Allow the user to create three passwords at once.
--- /task ---

--- task ---
Add this code to create three passwords.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 8
---
import random

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'

length = input('password length?')
length = int(length)

for p in range(3):
password = ''
for c in range(length):
    password += random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
Indent the code for creating a password so that it repeats three times.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 9-12
---
import random

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'

length = input('password length?')
length = int(length)

for p in range(3):
    password = ''
    for c in range(length):
        password += random.choice(chars)
    print(password)
--- /code ---
</div>

--- task ---
**Test:** Click the **Run** button.

You should now see three passwords of your chosen password length.
--- /task ---
