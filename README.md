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

