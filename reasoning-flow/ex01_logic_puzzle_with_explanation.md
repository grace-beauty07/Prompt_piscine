# Objective: Guide the model to solve a problem with explicit reasoning.
-----
## Prompt 1: "Alex is x years old mother is twice his age. In 5 years Alex mother would be 40. How old is Alex mother."
## Output:
>### Alex is *x* years old.
>### His mother is twice his age, so her age is *2x*.
>### We’re told that in 5 years, Alex’s mother will be 40.
>### So we set up the equation:
>### 2x + 5 = 40
>### Because her current age (2x) plus 5 years equals 40.
>### Now solve it:
>### 2x = 35
>### x = 17.5
>### So Alex is 17.5 years old. Yes, that half year matters. Humans age continuously. We just round for convenience.
>### Now find the mother’s age:
>### 2x = 2 × 17.5 = 35
>### So Alex’s mother is *35 years old*.
>### Check it:
>### 35 + 5 = 40.
-----
## Prompt 2: "Explain your reasoning before giving the final answer."
## Output:
### Step 1:
>### Let Alex’s age be x.
### Step 2:
>### His mother is twice his age.
>### Mother’s age = 2x.
### Step 3:
>### In 5 years, his mother will be 40.
>### So we add 5 to her current age:
>### 2x + 5 = 40
### Step 4:
>### Solve the equation:
>### 2x + 5 = 40
>### 2x = 40 − 5
>### 2x = 35
>### x = 17.5
### Step 5:
>### Find the mother’s age now:
>#### 2 × 17.5 = 35
### Final Answer:
>### Alex’s mother is 35 years old.
-----
## Verification of reasoning:
>### Yes, the model provided step by step reasoning before the final answer