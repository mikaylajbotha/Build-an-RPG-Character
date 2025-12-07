# Build an RPG Character

In this lab you will practice the basics of Python by building a small app that creates a character for an RPG adventure.

---

## Objective

Fulfill the user stories below and get all the tests to pass to complete the lab.

---

## User Stories

- You should have a function named `create_character`.
- The function should accept, in order, a character name followed by three stats: **strength**, **intelligence**, and **charisma**.

### Character Name Validation

The character name should be validated:

1. If the character name is not a string, the function should return:  
   `"The character name should be a string."`
2. If the character name is longer than 10 characters, the function should return:  
   `"The character name is too long."`
3. If the character name contains spaces, the function should return:  
   `"The character name should not contain spaces."`

### Stats Validation

The stats should also be validated:

1. If one or more stats are not integers, the function should return:  
   `"All stats should be integers."`
2. If one or more stats are less than 1, the function should return:  
   `"All stats should be no less than 1."`
3. If one or more stats are more than 4, the function should return:  
   `"All stats should be no more than 4."`
4. If the sum of all stats is different than 7, the function should return:  
   `"The character should start with 7 points."`

---

## Character Sheet Output

If all values pass validation, the function should return a string with four lines:

1. The first line should contain the character name.
2. Lines 2-4 should start with the stat abbreviation, **STR**, **INT**, or **CHA** (in this order), followed by a space, and then a number of full dots (`●`) equal to the value of the stat, and a number of empty dots (`○`) to reach 10.

**Example:**

Note: While str and int are common abbreviations for the stats, they are reserved keywords in Python and should not be used as variable names.

Tests Passed

You should have a function named create_character. ✅

When create_character is called with a first argument that is not a string it should return "The character name should be a string." ✅

When create_character is called with a first argument that is longer than 10 characters it should return "The character name is too long." ✅

When create_character is called with a first argument that contains a space it should return "The character name should not contain spaces." ✅

When create_character is called with a second, third or fourth argument that is not an integer it should return "All stats should be integers." ✅

When create_character is called with a second, third or fourth argument that is lower than 1 it should return "All stats should be no less than 1." ✅

When create_character is called with a second, third or fourth argument that is higher than 4 it should return "All stats should be no more than 4." ✅

When create_character is called with a second, third or fourth argument that do not sum to 7 it should return "The character should start with 7 points." ✅

create_character("ren", 4, 2, 1) should return:

ren
STR ●●●●○○○○○○
INT ●●○○○○○○○○
CHA ●○○○○○○○○○
``` ✅  

10. When `create_character` is called with valid values it should output the character stats as required. ✅


```text
ren
STR ●●●●○○○○○○
INT ●●○○○○○○○○
CHA ●○○○○○○○○○
