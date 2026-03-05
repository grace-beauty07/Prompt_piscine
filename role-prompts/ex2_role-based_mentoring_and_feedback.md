# Objective: Use role-based prompts for personalized feedback.
# Code
```python
name = input('what is your name?: ')
food = input('what is your favorite food?: ')

message = f(' {name} said her favorite food is {food}')
print(message)
```

# Mentor role:
>## First, here’s your original line that causes trouble:
```python
message = f('{name} said her favorite food is {food}')
```
>## That’s not how f-strings work. You don’t wrap the string in parentheses like a function call. Python isn’t a vending machine where you insert f() and get formatting out.
>## Corrected version:
```python
name = input('What is your name? ')
food = input('What is your favorite food? ')

message = f"{name} said her favorite food is {food}."
print(message)
```
-----
# 3. Response Review
>## Yes, the assigned role absolutely influenced the feedback style.
>## The response was technically correct. The syntax fix was accurate. The improvements were reasonable. The teaching progression was logical. From a purely instructional standpoint, it worked.
>## Stylistically The “mentor” role clearly shaped the tone.
