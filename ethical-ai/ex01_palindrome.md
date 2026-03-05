# Objective: Experience the difference between using AI as a shortcut and using it as a learning tool.

## Step 1 - Do it yourself
>### 1. Write a pseudocode for a function that checks if a string is a palindrome.
>### 2. Implement your solution in Python.
>### 3. Test with examples like "racecar", "hello", and "A man a plan a canal Panama".
>### 4. Add comments explaining your reasoning.

## Step 2 - Use AI to learn
 ### Now that your function works, use AI to go deeper:
>- #### "I wrote a palindrome function. Here's my code:[insert your code]
>- #### What's the time complexity?
>- #### What edge cases might I miss?
>- #### Are there better approaches?"

## Step 3 - Reflection
>- ### What did you learn from solving it before asking AI?
>- ### How is your understanding different now?
>- ### Could you now write similar functions (e.g., reverse a string) without help?


# Step One: Do it yourself

## *Pseudocode For A Function That Checks If A String Is A Palindrome:*
### Step 1: define/declare the funtion (isPalindrome).
### Step 2: find the length of the string.
### Step 3: compare the characters on the left side of the string with the characters on the right side of the string using a for loop $ if statement.
### Step 4: if the character on the left side of the string doesn't correspond with the character on the right side of the string return false, if it does return true.

## *Python Solution:*
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
## *Examples:*
| Input | Output |
| :-----: | :-----: |
| "racecar" | True |
| "hello" | False |
| "A man a plan a canal Panama" | False |


# Step Two: AI learning
### What's the time complexity?
> O(n)
### What edge cases might I miss?
>  Empty string, spacing and punctuations, case sensitivity etc.
### Are there better approaches?
> Yes, there are


# Step Three: Reflection
### What did you learn from solving it before asking AI?
> I learnt how to write some python synthax (I didn't know how to do that before)
### How is your understanding different now?
> It has improved
### Could you now write similar functions (e.g., reverse a string) without help?
> Yes I can (though,I'll need to do a lot of research)
