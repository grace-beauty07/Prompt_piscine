# Objective: Use structured prompting to encourage reasoning.
-----
## Prompt without reasoning: "What is the LCM of 120 and 240?"
## Output:
>- ### The LCM of 120 and 240 is *240*.
-----
## Prompt with reasoning: "Let's think step by step. What is the LCM of 120 and 240?"
## Output:
### Step 1: Prime factorize both numbers;
>### 120 = 2³ × 3 × 5
>### 240 = 2⁴ × 3 × 5
### Step 2: Take the highest power of each prime that appears;
>### 2⁴, 3¹, 5¹
### Step 3: multiply them;
>### 2⁴ × 3 × 5
>### = 16 × 3 × 5
>### = 48 × 5
>### = 240

### Final answer:
>### LCM of 120 and 240 = *240*.
-----
## Comparison of output:
>### The first one gives the direct answer while the second one gives a step by step solution before the answer
