<h2 class="c-project-heading--task">Lots of passwords</h2>

Use a **loop** to allow the user to create several passwords at once.

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

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?1234567890'  # Characters the password can use

length = input('Password length?')   # Ask how long each password should be
length = int(length)                 # Convert the input into a whole number

for p in range(3):                   # Repeat three times to make three passwords
    password = ''                    # Start with an empty password
    for c in range(length):          # Build one password character by character
        password += random.choice(chars)
    print(password)                  # Show each completed password

--- /code ---
</div>
### Tip

<div class="c-project-callout c-project-callout--tip">

Make sure that the lines beneath your `for` loop keep the same indentation when you **nest** them!

</div>

## Now run your code

Click on **Run**.

Enter a number when asked.

You should see **three passwords**, each the length you chose.
