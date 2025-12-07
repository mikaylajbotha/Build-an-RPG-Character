# Build-an-RPG-Character
-Python Practice

# RPG Character Creator

A small Python app to create a character for an RPG adventure. This project practices basic Python skills including functions, conditionals, and string formatting.  

## Objective
Create a function `create_character` that validates character input and returns a formatted character sheet.  

--
## Function: `create_character(name, strength, intelligence, charisma)`

### Character Name Validation
- Must be a string → otherwise return: `"The character name should be a string."`  
- Max 10 characters → otherwise return: `"The character name is too long."`  
- No spaces → otherwise return: `"The character name should not contain spaces."`  

### Stats Validation
- All stats must be integers → otherwise return: `"All stats should be integers."`  
- Each stat must be ≥ 1 → otherwise return: `"All stats should be no less than 1."`  
- Each stat must be ≤ 4 → otherwise return: `"All stats should be no more than 4."`  
- Stats must sum to 7 → otherwise return: `"The character should start with 7 points."`  

### Character Sheet Format
- Returns a string with 4 lines:
  1. Character name  
  2. Strength (STR) bar: full dots (`●`) = stat value, empty dots (`○`) = 10 - stat value  
  3. Intelligence (INT) bar  
  4. Charisma (CHA) bar  

Example:
ren
STR ●●●●○○○○○○
INT ●●○○○○○○○○
CHA ●○○○○○○○○○


> **Note:** Avoid using `str` or `int` as variable names since they are reserved keywords in Python.  

---

## How to Run
1. Implement the `create_character` function in `main.py`.  
2. Call the function with the desired character name and stats.  
3. The function returns either a validation message or a formatted character sheet.  

---

## Tests
The following scenarios are tested:  
1. Function exists  
2. Name is not a string  
3. Name too long (>10 chars)  
4. Name contains spaces  
5. Stats are not integers  
6. Stats less than 1  
7. Stats greater than 4  
8. Stats do not sum to 7  
9. Correct format output for valid stats  
10. All valid inputs produce a formatted character sheet  

---

## Example Usage

```python
from main import create_character

character = create_character("ren", 4, 2, 1)
print(character)


> **Note:** Avoid using `str` or `int` as variable names since they are reserved keywords in Python.  

---

## How to Run
1. Implement the `create_character` function in `main.py`.  
2. Call the function with the desired character name and stats.  
3. The function returns either a validation message or a formatted character sheet.  

---

## Tests
The following scenarios are tested:  
1. Function exists  
2. Name is not a string  
3. Name too long (>10 chars)  
4. Name contains spaces  
5. Stats are not integers  
6. Stats less than 1  
7. Stats greater than 4  
8. Stats do not sum to 7  
9. Correct format output for valid stats  
10. All valid inputs produce a formatted character sheet  

---

## Example Usage

```python
from main import create_character

character = create_character("ren", 4, 2, 1)
print(character)
