# Objective: Practice designing prompts that mimic function calls.
---
# Create a prompt:
## Prompt: Simulate a weather API response for Paris today.
## Model output:
```json
{
  "location": {
    "city": "Paris",
    "country": "FR",
    "latitude": 48.8566,
    "longitude": 2.3522
  },
  "date": "2026-02-19",
  "weather": {
    "condition": "Partly Cloudy",
    "description": "Cool with intermittent sunshine",
    "temperature": {
      "current": 9,
      "feels_like": 7,
      "min": 5,
      "max": 12,
      "unit": "C"
    },
    "humidity": 76,
    "wind": {
      "speed": 14,
      "direction": "NW",
      "unit": "km/h"
    },
    "pressure": 1018,
    "visibility": 10,
    "uv_index": 2
  },
  "sun": {
    "sunrise": "07:58",
    "sunset": "18:02"
  },
  "forecast_summary": "Mild winter day with light winds and occasional cloud cover."
}
```
---
# JSON schema:
## Prompt: Simulate a weather API response for Paris today. Expected format:
```json
{
      "location": "Paris",
      "temperature_celsius": 18,
      "condition": "Cloudy"
    }
```
## Model output:
```json
{
  "location": "Paris",
  "temperature_celsius": 18,
  "condition": "Cloudy"
}
```
---
# Testing with different cities:
## Prompt: Simulate a weather API response for Accra, New York and Pretoria today. Expected format:
```json
{
      "location": "Paris",
      "temperature_celsius": 18,
      "condition": "Cloudy"
    }
```
## Model output:
```json
[
  {
    "location": "Accra",
    "temperature_celsius": 31,
    "condition": "Sunny"
  },
  {
    "location": "New York",
    "temperature_celsius": 6,
    "condition": "Partly Cloudy"
  },
  {
    "location": "Pretoria",
    "temperature_celsius": 24,
    "condition": "Thunderstorms"
  }
]
```
---
# Comparison:
>## The outputs are similar but the data is different
