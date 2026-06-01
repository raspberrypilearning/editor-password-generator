<h2 class="c-project-heading--task">Choose a password length</h2>

Allow the user to choose how long their password should be.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 5-6,10
---
import random   # Import tools for choosing random items

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?1234567890'  # Characters the password can use

length = input('Password length?')   # Ask the user how long the password should be
length = int(length)                 # Convert the input into a whole number

password = ''                        # Start with an empty password

for c in range(length):              # Repeat as many times as the user chose
    password += random.choice(chars) # Add one random character each time

print(password)                      # Show the final password

--- /code ---
</div>

### Tip

<div class="c-project-callout c-project-callout--tip">

Make sure that the line beneath your `for` loop is indented with four spaces.

</div>

## Now run your code

Click on **Run**.

Enter a number when asked.

The password that is printed should be exactly that length.
