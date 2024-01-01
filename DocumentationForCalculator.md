# Documentation for Valerie's Math Machine
Valerie's Math Machine is a simple calculator that can help users solve arithmetic problems. 

## Constants

*Note: There aren't explicit constants declared using the `const` keyword as constants in JavaScript. However, my code uses an object named `calculator` to maintain the state of the calculator, which acts as a sort of constant throughout the script. This object holds various properties.*

### Calculator

#### Properties

- **displayValue**  
Represents the value displayed on the calculator screen.  
- **firstOperand**  
Holds the first operand for arithmetic operations.  
- **waitingForSecondOperand**  
A boolean flag indicating whether the calculator is waiting for the second operand.  
- **operator**  
Stores the operator (+, -, *, /) for arithmetic calculations.  

## Functions
These functions work together to handle user interactions with the calculator and to update the display accordingly.

### calculate(firstOperand, secondOperand, operator)  
Performs arithmetic operations based on the provided operator and two operands.  

#### Parameters

- **firstOperand**  
The first number in the arithmetic operation  
- **secondOperand**  
The second number in the arithmetic operation  
- **operator**  
The arithmetic operator  

### handleOperator(nextOperator)  
Handles the selection of an operator (+, -, *, /). It performs operations based on the selected operator and updates the calculator's state accordingly.  

#### Parameter
- **nextOperator**  
The arithmetic operator (+, -, *, /) that has been selected

### inputDigit(digit)  
Appends the provided digit to the display value on the calculator screen.  

#### Parameter
- **digit**  
The digit to be added to the calculator's display  

### inputDecimal(dot)  
Handles the input of the decimal point ('.') and prevents multiple decimal points in a number.

#### Parameter
- **dot**  
The decimal point ('.') to be added to the display

### resetCalculator
Resets the calculator to its initial state, clearing the display and resetting operand values.  

### updateDisplay
Updates the calculator screen with the current display value.  

### Event Listener (Anonymous Function)  
This anonymous function attached to the `.calculator-keys` element listens for button clicks. It identifies the clicked button, determines the action based on the button value, and calls the respective functions or updates the display.