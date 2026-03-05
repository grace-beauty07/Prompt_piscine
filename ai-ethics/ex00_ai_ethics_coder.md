# Objective: Understand the fundamental difference between using AI to get answers vs. using AI to learn and develop irreplaceable skills.
# Part A: Self Assessment;

## Read and reflect: AI can already code. It can generate functions, debug syntax, and implement algorithms in seconds. This means:

## If your only skill is writing code that AI can write, you are already replaceable. The question is not whether to use AI. The question is how to use it.

## 1. Write down your honest answers:

> ### - How have you used AI for coding so far?
>ans: I copy and paste the problems on AI then I copy and paste the solution.
> ### - Do you ask AI for solutions before trying yourself?
>ans: Usually, I don't.
> ### - Can you explain code you've submitted without AI's help?
>ans: There is no code that I've submitted without the help of AI.

## 2. What would happen if AI was suddenly unavailable during an exam or interview?

## Identify your current pattern:
### Which learner are you now?:
>#### Learner A: "AI is my answer generator"
>#### Asks: "Write a function that does X"
>#### Copies code without reading carefully
>#### Moves on once it works
>#### Cannot explain how the code works


# Part B: Palindrome Solution + Reflection

## Challenge: Implement a simple function to check if a string is a palindrome.

# Step 1: Attempt independently
## Write pseudocode for a palindrome check:
>### Step 1: define/declare the funtion (isPalindrome).
>### Step 2: find the length of the string.
>### Step 3: compare the characters on the left side of the string with the characters on the right side of the string using a for loop & if statement.
>### Step 4: if the character on the left side of the string doesn't correspond with the character on the right side of the string return false, if it does return true.
## Implement your solution in Python:
```python
# Define the function
 def isPalindrome(str):
     # Check the length of the string
     length = len(str)
     # Loop through the string to check each character from index zero to the midpoint
     for i in range(0, length // 2):
        # Check for a character that isn't mirrored around the center
        if (str[i] != str[length - i - 1]):
            return False
     return True

# This solution discovers false Palindromes by checking that the first half of the characters are mirrored on the other side of the string
```
## Test with examples: racecar, hello, A man a plan a canal Panama:
| Input | Output |
| :-----: | :-----: |
| "racecar" | True |
| "hello" | False |
| "A man a plan a canal Panama" | False |
## Debug any issues yourself:
>### When I tested with the last example the output was false instead of true and the reason is my code is not case sensitive.

# Step 2: Strategic AI Use:
>## Edge cases I missed:
>### 1. Non-letters on the left can break alignment
>### This line:
```python
if not str[i].isalpha():
    continue
```
>### 2. It can crash on strings with only symbols
>### Example:
>### "!!!"
>### This part:
```python
while not str[j].isalpha():
    j -= 1
```
>### 3. It ignores numbers
>### Because I used .isalpha(), this:
>### "12321", Will return True immediately (no comparisons happen).
>### If I want numbers included, I should use:
```python
.isalnum()
```
>### 4. Using str as a variable name
>### Minor but important:
```python
def isPalindrome(str):
```
>### str is a built-in type in Python.
>### Better:
```python
def is_palindrome(s):
```
>- ### After writing and testing my solution, I used AI to analyze my function by checking for time complexity, identifying possible edge cases and how it performs on very long strings. All this gave me more insight.

# Step 3: Reflection
>## What did you learn by struggling first?
>- ### I learnt how to write some python synthax (I didn't know how to do that before)
>## How is your understanding different than if you'd just asked for the solution?
>- ### It has improved
>## Can you now implement similar functions (reverse a string, find duplicates) without AI?
>- ### Yes I can (though,I'll need to do a lot of research)
>## What mental modelYes I can (though,I'll need to do a lot of research) did you build?
>- ### Using reverse string to solve the problem

# Part D: The Fairness Contract
>## I will use AI:
>- ### After I've attempted a problem for at least 20 minutes
>- ### To understand why my solution works/doesn't
>- ### To explore alternatives after I have a working solution
>- ### [add your rules]:
>- ### To understand what my solution does and tolook at other examples
>## I will NOT use AI when:
>- ### I haven't tried the problem myself
>- ### I'm taking an assessment or test
>- ### I need to build fundamentals
>- ### [add your rules]:
>- ### I have not done my own research
>## I know I'm using AI fairly when:
>- ### I can explain my code without looking at AI's response
>- ### I could solve similar problems without AI
>- ### I feel more confident in my abilities
>- ### [add your rules]:
>- ### I am able to build fundamentals
>## Sign and date this contract:
>- ### *Signature: Grace Kalu*
>- ### *Date: Thursday 12th February 2026*

# Part E: Scenario Analysis

>## Interview: "Explain how you'd implement a caching system." If you always relied on AI, can you answer?
>- ### *If I have always relied on AI, I can't answer*
>## Production bug at 2 AM: AI is unavailable. Can you debug code you don't fully understand?
>- ### *NO*
>## New tech with little documentation: If you never learned to read docs and experiment, what happens?
>- ### *I would struggle*
>## Write a paragraph: How does using AI fairly now prepare you for these scenarios?
>- ### *If I use AI fairly, I will get to really understand what I'm doing, this will build my level of confidence because I know that being confident gives you and edge during interviews. Also, I will remain relevant and irreplaceable in any field*

# Part F: Skills Assessment + Action Plan

## Rate yourself 1–5 and write an improvement plan for your lowest area:

>### Problem decomposition 3/5
>### Systems thinking 5/5
>### Critical evaluation 1/5
>### Debugging mindset 1/5
>### Conceptual understanding (the "why") 5/5

## Action plan: 3 specific actions this week to improve it without outsourcing thinking to AI:
## I plan to:
>### do more indept research
>### practice intensly
>### network vigorously
