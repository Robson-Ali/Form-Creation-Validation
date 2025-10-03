# Form-Creation-Validation
A simple user registration form project that demonstrates form creation and client-side validation using HTML, CSS, and vanilla JavaScript.

## Project Overview
This repository contains a user registration form where users enter a username, email, and password. The form implements basic validation rules using plain JavaScript to ensure data correctness before submission:

- Username: Minimum 3 characters.
- Email: Must contain '@' and '.' characters.
- Password: Minimum 8 characters.
- Users receive live feedback below the form if the inputs do not meet these requirements, or a success message when validation passes.

## Task Requirements
### Setup and Initial Code Structure
1. Start with DOMContentLoaded Event:

2. Wrap your entire script in a DOMContentLoaded event listener. This ensures your JavaScript runs after the entire HTML document has been loaded.
Form Selection:

3. Use document.getElementById to select the form with id="registration-form". Store this reference in a constant named form.
Feedback Division Selection:

4. Similarly, select the division where feedback will be displayed (id="form-feedback") and store it in a constant named feedbackDiv.
4.1 Form Submission and Event Prevention
4.2 Form Submission Event Listener:
4.3 Add an event listener to form for the ‘submit’ event. Use an anonymous function to handle the event.
4.4 Inside this function, call event.preventDefault() to prevent the form from submitting to the server. This is crucial for client-side validation.
4.5 Input Retrieval and Trimming
4.6 Retrieve User Inputs:
4.7 Use document.getElementById to select each input field by its respective ID: username, email, and password.
4.8 For each, retrieve the .value property and apply the .trim() method to remove any leading or trailing whitespace. Store these trimmed values in constants named after each input field.
4.9 Validation Logic
4.10 Initialize Validation Variables:

5. Declare a variable named isValid and set it to true. This will track the overall validation status.
6. Declare an array named messages to store validation error messages.
7. Username Validation:
7.1 Check if username.length is less than 3. If so, set isValid to false and add a specific error message to messages.
Email Validation:
7.2 Check if email includes both ‘@’ and ‘.’ characters. If not, set isValid to false and append a corresponding error message to messages.
Password Validation:
7.3 Ensure password.length is at least 8. If it falls short, update isValid to false and add an appropriate error message to messages.
8. Displaying Feedback
8.1 Feedback Display Logic:
8.2 Make feedbackDiv visible by setting its style.display to "block".
8.3 If isValid remains true, set the textContent of feedbackDiv to "Registration successful!" and its style.color to "#28a745".
8.4 If isValid is false, join messages with <br> to form a single string, and assign this to the innerHTML of feedbackDiv. Set feedbackDiv.style.color to "#dc3545".

## Files Structure
* index.html – Contains the HTML markup for the registration form.
* style.css – Styles for the form layout and feedback messages.
* script.js – JavaScript file implementing form validation logic.

## Setup Instructions
Clone the repository:

### text
git clone https://[github.com/Robson-Ali/Form-Creation-Validation.git](https://github.com/Robson-Ali/Form-Creation-Validation)
Open index.html in your preferred browser.

## Fill out the form fields and submit to see validation in action.

### Validation Details
* JavaScript code is wrapped inside a DOMContentLoaded event listener to ensure the DOM is fully loaded before scripts run.
* Form submission is intercepted using event.preventDefault() to handle validation without page reload.

### Validation logic checks:
* Username length (at least 3 characters)
* Email contains @ and .
* Password length (at least 8 characters)
* Feedback messages are dynamically displayed in the #form-feedback div:
* Valid submission shows a green success message.
* Invalid inputs show red error messages.

## Technologies Used
* HTML5
* CSS3
* JavaScript (vanilla ES6+)

## Contribution
Feel free to fork this repository and submit pull requests with improvements or additional validation rules.
