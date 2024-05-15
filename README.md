# Calories Counter App

This application is designed to help you track your daily caloric intake and manage your dietary goals with ease.

## Project Overview:

The Calorie Counter App is a web-based tool developed using HTML, CSS, and JavaScript. It allows users to input their daily caloric budget and log their meals and exercises throughout the day. The app then calculates the remaining calories based on the inputs provided, helping users stay on track towards their health and fitness goals.

## JavaScript Logic Explanation:

The Calorie Counter App's JavaScript code consists of several functions and event listeners that handle user interactions, input validation, and calculations. Here's a breakdown of the key JavaScript logic:

### 1. Event Listeners Setup:

The JavaScript code starts by selecting various HTML elements from the DOM using document.getElementById() and document.querySelector(). Event listeners are then attached to specific elements to trigger actions when certain events occur, such as clicking buttons or submitting forms.

### 2. Input Validation Functions:

Two main functions handle input validation:

- cleanInputString(str): This function removes any non-numeric characters from a string, ensuring that only valid numeric inputs are processed.

- isInvalidInput(str): This function checks if a string contains invalid input, such as exponential notation (e.g., 1e3). If invalid input is detected, an alert is displayed to notify the user.

### 3. Adding Entries

The addEntry() function is called when the user clicks the "Add Entry" button. It dynamically generates HTML input fields for the selected entry type (e.g., breakfast, lunch) and appends them to the corresponding fieldset container in the form.

### 4. Calculating Calories

The calculateCalories(e) function is invoked when the user submits the form to calculate remaining calories. This function retrieves input values from various HTML input elements, calculates consumed and remaining calories, and updates the output display accordingly.

### 5. Helper Functions:

- getCaloriesFromInputs(list): This function iterates over a list of HTML input elements, extracts their values, performs input validation, and calculates the total calories. It returns the sum of valid input values or null if invalid input is detected.

### 6. Clearing Form

The clearForm() function resets the form by clearing all input fields and hiding the output display.
