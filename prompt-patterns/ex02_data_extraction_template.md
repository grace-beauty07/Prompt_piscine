# Objective: Extract structured data from unstructured input.

    Choose an unstructured text (e.g., "John Doe, age 29, lives in Paris and works as a software engineer.").

    Create a template prompt:

        "Extract the following fields from the text: Name, Age, Location, Occupation. Return the output in JSON format."

    Validate the output and ensure consistency across multiple inputs.

## Unstructured text:
>### Bessie, age 27, lives in London and works as a barber at Mastercut Salon
-----
## Prompt:
>### Extract the following fields from the text: Name, Age, Location, Occupation, Company name. Return the output in JSON format. Bessie, age 27, lives in London and works as a barber at Mastercut Salon
## Output:
 ```json
 {
  "Name": "Bessie",
  "Age": 27,
  "Location": "London",
  "Occupation": "Barber",
  "Company name": "Mastercut Salon"
 }
```
-----
# Validation across multiple inputs:
## Prompt:
>### Extract the following fields from the text: Name, Age, Location, Occupation, Company name. Return the output in JSON format. Ololade Bankole, age 37, lives in Abuja and works as a Chef at Smallville Hotel Nkechi Umeh, age 65, lives in Lagos and works as a teacher at Queensland Private School Itunu Oni, age 70, lives in Paris and works as a Coding Mentor at Learn2Earn Jesus Navas, age 65, lives in Spain and works as a footballer at PSG
## Output:
```json
[
  {
    "Name": "Ololade Bankole",
    "Age": 37,
    "Location": "Abuja",
    "Occupation": "Chef",
    "Company name": "Smallville Hotel"
  },
  {
    "Name": "Nkechi Umeh",
    "Age": 65,
    "Location": "Lagos",
    "Occupation": "Teacher",
    "Company name": "Queensland Private School"
  },
  {
    "Name": "Itunu Oni",
    "Age": 70,
    "Location": "Paris",
    "Occupation": "Coding Mentor",
    "Company name": "Learn2Earn"
  },
  {
    "Name": "Jesus Navas",
    "Age": 65,
    "Location": "Spain",
    "Occupation": "Footballer",
    "Company name": "PSG"
  }
]
```
### The input works perfectly across multiple inputs
