# Documentation for Valerie's Math Machine
Valerie's Math Machine is a simple calculator that can help users solve basic arithmetic problems. 

## Constants

### Calculator

DRAFT TEXT
There aren't explicit constants declared using the const keyword as constants in JavaScript. However, my code uses an object named calculator to maintain the state of the calculator, which acts as a sort of constant throughout the script. This object holds various properties:

    displayValue: Represents the value displayed on the calculator screen.
    firstOperand: Holds the first operand for arithmetic operations.
    waitingForSecondOperand: A boolean flag indicating whether the calculator is waiting for the second operand.
    operator: Stores the operator (+, -, *, /) for arithmetic calculations.



## Functions
These functions work together to handle user interactions with the calculator, processing input, performing calculations, and updating the display accordingly.

### calculate

### handleOperator

### inputDigit

### inputDecimal

### resetCalculator

### updateDisplay

DRAFT TEXT FOR FUNCTIONS
    inputDigit(digit): Appends the provided digit to the display value on the calculator screen.

    inputDecimal(dot): Handles the input of the decimal point ('.') and prevents multiple decimal points in a number.

    handleOperator(nextOperator): Handles the selection of an operator (+, -, *, /). It performs operations based on the selected operator and updates the calculator's state accordingly.

    calculate(firstOperand, secondOperand, operator): Performs arithmetic operations based on the provided operator and two operands.

    resetCalculator(): Resets the calculator to its initial state, clearing the display and resetting operand values.

    updateDisplay(): Updates the calculator screen with the current display value.

    Event Listener Function: The anonymous function attached to the .calculator-keys element listens for button clicks. It identifies the clicked button, determines the action based on the button value, and calls the respective functions (handleOperator, inputDecimal, resetCalculator, inputDigit) or updates the display (updateDisplay).

NOTES ON PARAMETERS

        inputDigit(digit): Takes a single parameter digit, representing the digit to be added to the calculator's display.

        inputDecimal(dot): Accepts a single parameter dot, representing the decimal point ('.') to be added to the display.

        handleOperator(nextOperator): Receives a single parameter nextOperator, representing the arithmetic operator (+, -, *, /) that has been selected.

        calculate(firstOperand, secondOperand, operator): Takes in three parameters: firstOperand (the first number in the arithmetic operation), secondOperand (the second number in the operation), and operator (the arithmetic operator).

        These functions utilize these parameters to perform specific tasks or calculations based on the values passed to them when they are invoked elsewhere in the code. The parameters allow these functions to receive and work with different values dynamically, enabling the calculator's functionality based on user input.


FUNCTION DOCUMENTATION TEMPLATE
## getDirections(latitude, longitude, directionsCallback)
Returns the directions from the current location to the destination location.
- Parameters
    - latitude
    Type: Number
    Latitude of the destination, in degrees
    - longitude
    Type: Number
    Longitude of the destination, in degrees
    - directionsCallback
    Type: Function
    Called when the directions are returned from the server. Contains a string parameter named **directions**, which has the directions for how to travel from the current location to the destination.

