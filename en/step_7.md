<h2 class="c-project-heading--task">Choosing the number of passwords</h2>

--- task ---
Allow the user to choose how many passwords to generate.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 6-7,12
---
#!/bin/python3
import random   # Import tools for choosing random items

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'  # Characters the password can use

number = input('number of passwords?')   # Ask how many passwords to generate
number = int(number)                     # Convert the input into a whole number

length = input('password length?')       # Ask how long each password should be
length = int(length)                     # Convert the input into a whole number

for p in range(number):                  # Repeat for the number of passwords chosen
    password = ''                        # Start with an empty password
    for c in range(length):              # Build one password character by character
        password += random.choice(chars)
    print(password)                      # Show each completed password

--- /code ---
</div>

--- task ---
**Test:** Click **Run**.

Enter two numbers when asked.  
You should see the chosen number of passwords, each the length you selected.
--- /task ---
