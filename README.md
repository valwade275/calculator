# Calculator

This code represents a basic calculator implemented using HTML, CSS, and JavaScript. Here's a breakdown of its structure and functionality:

## HTML Structure

The HTML section defines the structure of the calculator using divs and buttons.
It includes a calculator screen (<input> element) and a set of buttons representing digits, operators (+, -, *, /), decimal point, and clear functionalities.

## CSS Styling

The CSS section styles the calculator's appearance, defining sizes, colors, button styles, and layout using classes like `.calculator`, `.calculator-screen`, `.calculator-keys`, etc.

## JavaScript Functionality

The JavaScript section handles the calculator's logic and functionality.
`calculator` is an object that holds the calculator's state, including the display value, operands, operator, and a flag indicating whether the calculator is waiting for a second operand.
Functions like `inputDigit`, `inputDecimal`, `handleOperator`, `calculate`, `resetCalculator`, and `updateDisplay` handle different aspects of the calculator's behavior.
Event listeners are attached to the calculator keys, allowing the calculator to respond to button clicks. Depending on the button clicked, it performs operations like inputting digits, handling decimals, operators, clearing the display, etc.
The `updateDisplay` function updates the calculator screen with the current display value.

## Overall Functionality

Users can click on the buttons to input digits, perform basic arithmetic operations, use the decimal point, clear the display, and get the result by pressing the "=" button.
The JavaScript functions handle these button clicks and update the display accordingly.
