Python User Registration System
Project Overview
This project is a complete, self-contained user registration system written in Python. It's designed to validate user input for a sign-up form, ensuring that the name, email, and password meet specific security and formatting criteria before an account is created.

The script includes robust error handling to provide clear feedback when validation fails.

Core Features
Name Validation: Ensures the name is a string and is longer than two characters.

Email Validation: Checks for a valid email format, including a username, an @ symbol, and an approved top-level domain (e.g., .com, .org, .edu).

Password Strength Validation: Enforces a strong password policy, requiring a minimum length of 8 characters, at least one capital letter, and at least one number.

Error Handling: Uses try...except blocks to catch validation errors and return user-friendly messages.

How It Works
The system is built around two main functions:

validate_user(name, email, password): This function calls three helper functions (validate_name, validate_email, validate_password). If any check fails, it raises a ValueError. If all checks pass, it returns True.

register_user(name, email, password): This function calls validate_user(). If validation is successful, it returns a dictionary containing the user's data. If a ValueError is raised, it catches the error and returns False.

How to Use
To use the script, you can run it directly from your terminal to see the example outputs, or import the register_user function into another Python file.

# To run the examples in the script:
# python user_registration.py

Skills Demonstrated
Python Programming

Modular Function Design

Data Validation and Sanitization

Error and Exception Handling (try...except, raise ValueError)

String Manipulation

Control Flow (if/else, loops)
