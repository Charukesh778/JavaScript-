ChatGPT 4o mini

Log in
You said:
JavaScript program 
ChatGPT said:
ChatGPT
Sure! What kind of JavaScript program are you interested in? Here are a few examples of what you might be looking for:

Basic Calculator:
A simple program to add, subtract, multiply, and divide numbers.

To-Do List:
A program to manage a list of tasks, allowing you to add and remove items.

Form Validation:
A script to validate user input in a web form.

Clock:
A real-time clock that displays the current time.

Weather App:
A program that fetches and displays weather information from an API.

Let me know which one interests you, or if you have another idea in mind!


You said:
Program 
ChatGPT said:
ChatGPT
Sure! Here’s a simple JavaScript program that implements a basic calculator which can add, subtract, multiply, and divide two numbers. This example includLog in
You said:
JavaScript program 
ChatGPT said:
ChatGPT
Sure! What kind of JavaScript program are you interested in? Here are a few examples of what you might be looking for:

Basic Calculator:
A simple program to add, subtract, multiply, and divide numbers.

To-Do List:
A program to manage a list of tasks, allowing you to add and remove items.

Form Validation:
A script to validate user input in a web form.

Clock:
A real-time clock that displays the current time.

Weather App:
A program that fetches and displays weather information from an API.

Let me know which one interests you, or if you have another idea in mind!


You said:
Program 
ChatGPT said:
ChatGPT
Sure! Here’s a simple JavaScript program that implements a basic calculator which can add, subtract, multiply, and divide two numbers. This example includes HTML fores HTML for input and buttons, and JavaScript for the logic.

HTML:
html
Copy code
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Basic Calculator</title>
    <style>
        .calculator {
            max-width: 200px;
            margin: 50px auto;
            padding: 20px;
            border: 1px solid #ddd;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .calculator input, .calculator button {
            width: 100%;
            margin: 5px 0;
            padding: 10px;
            font-size: 16px;
        }
    </style>
</head>
<body>
    <div class="calculator">
        <input id="num1" type="number" placeholder="Enter first number">
        <input id="num2" type="number" placeholder="Enter second number">
        <button onclick="calculate('+')">Add</button>
        <button onclick="calculate('-')">Subtract</button>
        <button onclick="calculate('*')">Multiply</button>
        <button onclick="calculate('/')">Divide</button>
        <h2 id="result">Result: </h2>
    </div>

    <script>
        function calculate(operator) {
            const num1 = parseFloat(document.getElementById('num1').value);
            const num2 = parseFloat(document.getElementById('num2').value);
            let result;
            
            if (isNaN(num1) || isNaN(num2)) {
                result = "Please enter valid numbers.";
            } else {
                switch (operator) {
                    case '+':
                        result = num1 + num2;
                        break;
                    case '-':
                        result = num1 - num2;
                        break;
                    case '*':
                        result = num1 * num2;
                        break;
                    case '/':
                        result = num2 !== 0 ? num1 / num2 : "Cannot divide by zero.";
                        break;
                    default:
                        result = "Invalid operator.";
                        break;
                }
            }

            document.getElementById('result').textContent = `Result: ${result}`;
        }
    </script>
</body>
</html>
