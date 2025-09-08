# Calorie Counter

A simple web app to track your daily calorie intake and exercise against a set calorie budget.

## Features
- Set a **daily calorie budget**.
- Add entries for:
  - Breakfast
  - Lunch
  - Dinner
  - Snacks
  - Exercise
- Dynamically add multiple food or exercise items.
- Calculate remaining calories based on your input.
- Clear all data with one click.


## How It Works
1. Enter your daily calorie **budget**.
2. Add meals or exercises using the **Add Entry** button and dropdown menu.
3. Press **Calculate Remaining Calories**:
   - Total food calories are subtracted from your budget.
   - Exercise calories are added back.
   - The app shows whether you are **within** or **over** your budget.
4. Use the **Clear** button to reset everything.

## Example Usage
- Budget: `2000`
- Breakfast: `400`
- Lunch: `600`
- Dinner: `700`
- Snacks: `200`
- Exercise: `300`

**Remaining Calories = 2000 - (400+600+700+200) + 300 = 400**

## Requirements
- A modern web browser (Chrome, Firefox, Edge).
- No external libraries required.

## Possible Improvements
- Save entries using **localStorage** so they persist after refresh.
- Add **nutritional info** (protein, carbs, fats).
- Provide **visual charts** for calorie distribution.
