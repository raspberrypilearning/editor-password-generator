<h2 class="c-project-heading--task">A random password</h2>

To improve your program, make it add random characters one at a time to create a longer password.

In this step, you will write all the code in one go. The comments explain how each line helps build the password.

<div class="c-project-code">
--- code ---
---
language: python
filename: main.py
line_numbers: true
line_number_start: 1
line_highlights: 5,7-8
---
import random   # Import tools for choosing random items

chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ!@£$%^&*().,?1234567890'   # Characters the password can use (letters, numbers, and symbols)

password = ''     # Start with an empty password

for c in range(10):     # Repeat 10 times
    password += random.choice(chars)    # Add one random character to the password each time

print(password)     # Show the final password

--- /code ---
</div>

## Now run your code

Click on **Run**.

You should see a password that is 10 characters long. 
 
Try changing the number `10` to a bigger number, then run your code again to see how the password changes.
