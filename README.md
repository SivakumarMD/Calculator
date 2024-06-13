
# Calculator

This is a basic calculator web application with basic arithmetic operations, memory functions, and additional functionalities like square root, percentage, and reciprocal operations. The calculator features a responsive and visually appealing design.

## Features

- **Basic Arithmetic Operations**: Addition, subtraction, multiplication, and division.
- **Memory Functions**: Memory clear (MC), memory recall (MR), memory add (M+), and memory subtract (M-).
- **Additional Functions**: Square root (√), percentage (%), and reciprocal (1/x).
- **Clear Functions**: Clear last digit (CE) and clear all (AC).
- **Decimal Point Support**: Ability to handle decimal point numbers.
- **Responsive Design**: Adaptable to various screen sizes.

## Files

- `index.html`: The main HTML file containing the structure of the calculator.
- `styles.css`: The CSS file for styling the calculator. Note: The CSS is included in a `<style>` block within the HTML file for simplicity.

## HTML Structure

The `index.html` file includes:

- A `head` section with meta tags and inline CSS for styling.
- A `body` section with a calculator container (`div.calculator`) containing:
  - A display element (`div.calculator-display`) to show the current input and result.
  - Buttons for digits, operators, memory functions, and clear functions.

### Example HTML Structure

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Calculator</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        /* Inline CSS styling */
    </style>
</head>
<body>
    <div class="calculator">
        <div id="display" class="calculator-display">0</div>
        <button class="button memory-clear" onclick="memoryClear()">MC</button>
        <!-- Other buttons -->
    </div>
    <script src="script.js"></script>
</body>
</html>
```

## CSS Styling

Inline CSS is used for simplicity, focusing on:

- Centering the calculator.
- Applying a professional dark background color.
- Styling buttons, display, and other elements with appropriate colors, sizes, and effects.

### Example CSS

```css
body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #2c3e50;
    font-family: Arial, sans-serif;
}

.calculator {
    display: grid;
    grid-template-columns: repeat(5, 80px);
    gap: 10px;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
    background-color: #ecf0f1;
}

.calculator-display {
    grid-column: span 5;
    background-color: #34495e;
    color: #ecf0f1;
    font-size: 2.5rem;
    text-align: right;
    padding: 20px;
    border-radius: 10px;
    box-shadow: inset 0 0 10px rgba(0, 0, 0, 0.2);
    overflow-x: auto;
    white-space: nowrap;
}

/* Additional button styles */
```

## JavaScript Functionality

The `script.js` file includes:

- Variables to store the current input, operator, previous input, and memory.
- Functions for handling operations, number input, display updates, memory functions, and error handling.

### Example JavaScript

```javascript
let currentInput = '';
let operator = null;
let previousInput = '';
let shouldResetDisplay = false;
let memory = 0;

const displayElement = document.getElementById('display');

function chooseOperator(op) {
    // Functionality for choosing an operator
}

function appendNumber(number) {
    // Functionality for appending a number
}

function updateDisplay() {
    // Functionality for updating the display
}

// Additional functions
```

## Usage

1. **Download or clone the repository.**
2. **Open `index.html` in a web browser.**
3. **Use the buttons on the calculator for various arithmetic operations, memory functions, and additional features.**

## Author

- **Sivakumar M**
