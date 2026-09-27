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

Name: Aytunch Tuzdzhu
Contribution:
- Task 8
- Task 9

Design notes
------------
Main function boundaries:
- No outputs not used. Most functions only print the result so the data can't be further used.
- Used clear() function to make the UI clean. Though this cuts off the logs of previous commands.

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
- The program has a problem with error messages. For the functions get_number() and get_number_list(), you can type in an error message
  but it won't change depending on what actually makes the error. For example:

    damaged_parcels =  get_number("Damaged parcels: ", "Error - Value must be greater than zero.", int)
    
    Damaged parcels: 3.4
    -> Error - Value must be greater than zero. # Not the right error message since 3.4 > 0. The actual problem is that it's not an integer.

- The biggest limitation is that the data is not being used for anything. It's being printed but then cleared. 
  So if you wanted to save the data you'd have to write it down before proceeding.