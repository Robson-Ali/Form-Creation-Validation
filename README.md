# Form-Creation-Validation
A simple user registration form project that demonstrates form creation and client-side validation using HTML, CSS, and vanilla JavaScript.

## Project Overview
This repository contains a user registration form where users enter a username, email, and password. The form implements basic validation rules using plain JavaScript to ensure data correctness before submission:

* Username: Minimum 3 characters.
* Email: Must contain '@' and '.' characters.
* Password: Minimum 8 characters.
* Users receive live feedback below the form if the inputs do not meet these requirements, or a success message when validation passes.

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
