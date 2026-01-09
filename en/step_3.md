<h2 class="c-project-heading--task">Random characters</h2>

--- task ---
Create a program that chooses a random character for your password.
--- /task ---

--- task ---
Create a list of characters, stored in a variable called `chars`.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 3
line_highlights:
---
import random

chars = 'abcdefghijklmnopqrstuvwxyz'
--- /code ---
</div>

--- task ---
Choose a random character from the list, and store it in a variable called `password`.
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

chars = 'abcdefghijklmnopqrstuvwxyz'

password = random.choice(chars)
--- /code ---
</div>

--- task ---
Print your (very short!) password to the screen.
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

chars = 'abcdefghijklmnopqrstuvwxyz'

password = random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
**Test:** Click the **Run** button.

You should see a single random character on the screen.

If you run your program a few times, you should see different characters appear.
--- /task ---

--- task ---
Add some numbers to your `chars` variable to make the password more secure.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 3
---
import random

chars = 'abcdefghijklmnopqrstuvwxyz1234567890'

password = random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
**Test:** Click the **Run** button again a few times.  
You should sometimes see a number chosen.
--- /task ---
