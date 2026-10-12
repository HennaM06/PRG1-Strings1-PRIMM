# Task 2: Debugging, Part A, Answers

Complete this alongside `BRIEF_T2.md`.

## Fault log

### Fault 1

**What was wrong, and where**

> attempt != correct_pin:, i think this was wrong as when the pins match it reverses doing the opposite of what i want

**Why it caused incorrect behaviour, and how you fixed it**

> == tells python that the attempt must equal the original correct pin, if true the user can enter and if not it will be false

### Fault 2

**What was wrong, and where**

> while attempts_made <= MAX_ATTEMPTS: this means that the loop runs 4 times instead of the max of 3 attempts 

**Why it caused incorrect behaviour, and how you fixed it**

> while attempts_made < MAX_ATTEMPTS: this limits the attempts to the expected 3 therefore locking the system 

### Fault 3

**What was wrong, and where**

> print("Account locked. Too many incorrect attempts."), even after the correct password the account locked message still shows up

**Why it caused incorrect behaviour, and how you fixed it**

>     print("Account locked. Too many incorrect attempts.")
    By using a conditional, it will only run if the loop has finished without breaking 

### Fault 4

**What was wrong, and where**

>if check_pin(entered_pin, CORRECT_PIN):
    print("Access granted.")
Problem here is that even if the pin is correct, the loop continues to run as there isnt anything to stop it and so access granted is shown but asks for me pin attempts 

**Why it caused incorrect behaviour, and how you fixed it**

>     print("Access granted.")
    break
Adding break stops the loop after the correct pin has been entered.
