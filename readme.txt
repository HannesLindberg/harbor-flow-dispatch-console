HARBORFLOW DISPATCH CONSOLE - TEAM README

Run instructions
----------------
Command: python3 harborflow_app.py
Python version tested: Python 3.13.14

Team members and concrete contributions
---------------------------------------
Name: Hannes Lindberg
Contribution:
- Task 1
- Task 6
- Refactor code

Name: Hugo Karlsson
Contribution:
- Task 2
- Task 4
- Task 5

Name: Brian Rauch
Contribution: 
- Task 3
- Task 7

Nam: Aytunch Tuzdzhu
Contribution:
- Task 8
- Task 9

Design notes
------------
- Used clear() function to make the UI clean. 

Main function boundaries:
- No outputs not used. Most functions only print the result so the data can't be further used.

How input validation is organized:
- The validation checks the input with desired parameters and, if not valid, prints an error message and prompts the user again.
- Functions get_number() and get_number_list() are used to get inputs throughout the codebase. 
  The functions have integrated validation and can be adapted as wanted by changing the input arguments.
- Some validation does not have a helper due to the fact that they are only used once. For example: the validation for 
  service codes in task 3 is only used once and there is no need at the moment to make a helper function.

How shared calculations are reused:
- Calculation function for delivery quote calculate_delivery_quote() used in multiple tasks.
- Input functions get_number() and get_number_list() used for most input.

Known limitations
-----------------
There are no Limitations.

What we have done on Task 8:
- added try-except loop for service selecting part (Line 45-51)
- added while loop in Case 3 (Line 42-58)
- added while and try-except loop in Case 5 (Line 61-84)
- added while loop in case 6 (Line 84-104)
- added while loop in case 7 (Line 104-124)
- added while loop in case 8 (Line 200-219)