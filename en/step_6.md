<h2 class="c-project-heading--task">Lots of passwords</h2>

--- task ---
Allow the user to create several passwords at once using a **loop*.
--- /task ---

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 8-12
---
import random   # Import tools for choosing random items

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?0123456789'  # Characters the password can use

length = input('password length?')   # Ask how long each password should be
length = int(length)                 # Convert the input into a whole number

for p in range(3):                   # Repeat three times to make three passwords
    password = ''                    # Start with an empty password
    for c in range(length):          # Build one password character by character
        password += random.choice(chars)
    print(password)                  # Show each completed password

--- /code ---
</div>
<div class="c-project-callout c-project-callout--tip">

### Tip

- Make sure that the lines beneath your `for loop` keep the same indentation when you **nest** them!

</div>

--- task ---
**Test:** Click **Run**.

Enter a number when asked.  
You should see **three passwords**, each the length you chose.
--- /task ---
