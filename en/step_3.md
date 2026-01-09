<h2 class="c-project-heading--task">Using numbers and punctuation</h2>

--- task ---
Improve your program so that it can choose from capital letters, numbers, and punctuation.
--- /task ---

--- task ---
Add capital letters, numbers, and punctuation to your `chars` variable.
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

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'

password = random.choice(chars)
print(password)
--- /code ---
</div>

--- task ---
**Test:** Click the **Run** button.
--- /task ---
