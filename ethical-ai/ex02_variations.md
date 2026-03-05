# Objective: Extend your solution and practice independent problem-solving.

## 1. Modify your palindrome function to:
- ### Ignore spaces and punctuation.

- ### Be case-insensitive.

- ### Return the position where the string stops being a palindrome (if not one).

```python
def isPalindrome(str):
  length  = len(str)
  j = length - 1
  for i in range(0, length // 2):
    if not str[i].isalpha():
      continue
    
    while not str[j].isalpha():
      j -= 1
      
    if (str[i].lower() != str[j].lower()):
      
      return False
    
    j -= 1
  return True
```

## 2. After your first attempt, ask AI:

### "I modified my palindrome function to handle more cases.
### Did I miss anything?
>- ### Yes
### Can it be more efficient?"
>- ### Yes; below is a more efficient one:
```python
 def is_palindrome(s):
    i = 0
    j = len(s) - 1

    while i < j:

        # Skip non-letters on the left
        while i < j and not s[i].isalpha():
            i += 1

        # Skip non-letters on the right
        while i < j and not s[j].isalpha():
            j -= 1

        # Compare letters
        if s[i].lower() != s[j].lower():
            return False

        i += 1
        j -= 1

    return True
```

## 3. Reflect on what AI added that you didn't consider initially.
>- ### I didn't consider the risk of my code crashing or giving wrong results
