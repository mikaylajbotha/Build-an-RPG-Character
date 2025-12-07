# Build an RPG Character

This lab is part of the freeCodeCamp Python course. The goal is to practice Python basics by building a small application that creates a character for an RPG adventure.

---

## Objective

Create a function named `create_character` that:

1. Validates a character's name and stats.
2. Returns a properly formatted character sheet.
3. Passes all lab tests.

---

## User Stories

- The project must include a function named `create_character`.
- The function should accept, **in order**:
  1. `name` – the character's name.
  2. `strength` – integer between 1 and 4.
  3. `intelligence` – integer between 1 and 4.
  4. `charisma` – integer between 1 and 4.

---

## Character Name Validation

The character name must meet these criteria:

1. Must be a string. Otherwise, return:  
   `"The character name should be a string."`
2. Maximum 10 characters. Otherwise, return:  
   `"The character name is too long."`
3. Must not contain spaces. Otherwise, return:  
   `"The character name should not contain spaces."`

---

## Stats Validation

All three stats must be validated according to these rules:

1. Must be integers. Otherwise, return:  
   `"All stats should be integers."`
2. Minimum value of 1. Otherwise, return:  
   `"All stats should be no less than 1."`
3. Maximum value of 4. Otherwise, return:  
   `"All stats should be no more than 4."`
4. The sum of all stats must equal 7. Otherwise, return:  
   `"The character should start with 7 points."`

---

## Character Sheet Output

If all validations pass, the function should return a string formatted with four lines:

1. The first line contains the character's name.
2. Lines 2–4 display stats in this order: **STR**, **INT**, **CHA**.  
   Each line includes:
   - The stat abbreviation.
   - Full dots (`●`) equal to the stat value.
   - Empty dots (`○`) to fill up to 10 dots.

**Example:**

ren
STR ●●●●○○○○○○
INT ●●○○○○○○○○
CHA ●○○○○○○○○○

markdown
Copy code

> **Note:** `str` and `int` are reserved keywords in Python and should **not** be used as variable names.

---

## Tests Passed

1. Function `create_character` exists. ✅  
2. Name is not a string → returns `"The character name should be a string."` ✅  
3. Name longer than 10 characters → returns `"The character name is too long."` ✅  
4. Name contains spaces → returns `"The character name should not contain spaces."` ✅  
5. Stats are not integers → returns `"All stats should be integers."` ✅  
6. Stats less than 1 → returns `"All stats should be no less than 1."` ✅  
7. Stats greater than 4 → returns `"All stats should be no more than 4."` ✅  
8. Stats do not sum to 7 → returns `"The character should start with 7 points."` ✅  
9. `create_character("ren", 4, 2, 1)` returns the correctly formatted string:

ren
STR ●●●●○○○○○○
INT ●●○○○○○○○○
CHA ●○○○○○○○○○

yaml
Copy code
✅  
10. Valid inputs produce the character sheet exactly as required. ✅

---

## Summary

This lab helps practice:

- Python function definitions.
- Input validation (types, ranges, sums).
- String formatting.
- Handling multiple conditions and returning early on invalid input.
