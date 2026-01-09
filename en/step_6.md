```html
<h2 class="c-project-heading--task">Choosing a password length</h2>

--- task ---
Allow the user to choose the length of their password.
--- /task ---

--- task ---
Ask the user to input a password length, and store it in a variable called `length`.
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

length = input('password length?')

password = ''
for c in range(10):
    password += random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
Use `int()` to turn the user's input into a whole number.
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

length = input('password length?')
length = int(length)

password = ''
for c in range(10):
    password += random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
Use your `length` variable to repeat as many times as the user entered.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 9
---
import random

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'

length = input('password length?')
length = int(length)

password = ''
for c in range(length):
    password += random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
**Test:** Click the **Run** button.

The password created should be the length entered by the user.
--- /task ---
```
