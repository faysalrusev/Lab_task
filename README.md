# Lab_task
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script src="arrevennum.js"></script>
    <script src="arrmaxele.js"></script>
    <script src="calculator.js"></script>
    <script src="temperature.js"></script>
    

</body>
</html>


//Develop a simple calculator using JavaScript functions. 

function add(a, b) {
    return a + b;
}

function sub(a, b) {
    return a - b;
}

function multiply(a, b) {
    return a * b;
}

function div(a, b) {
    return a / b;
}

console.log(add(12, 11));      5
console.log(sub(14, 3));       
console.log(multiply(24, 3));  
console.log(div(100, 10));      


//Write a function convertToFahrenheit that converts Celsius         temperature to Fahrenheit.
Formula: Fahrenheit = (Celsius * 9/5) + 32


function fahrenheit(c) { 
    return (c * 9 / 5) + 32;
}

let c = parseFloat(prompt("Enter temperature in Celsius:"));
if (!isNaN(c)) {
    console.log(fahrenheit(c));
} else {
    console.log("Please enter a valid number.");
}


//Write a JavaScript program to find the largest number in an array.

let arr = [100, 303, 58, 210, 69];
let max = arr[0]; 

for (let i = 1; i < arr.length; i++) { 
    if (max < arr[i]) {
        max = arr[i];
    }
}

console.log("Maximum number is", max);

//Create a JavaScript function that returns an array of only the even numbers from an input array of numbers.


let arr = [7, 8, 9, 10, 11, 13];

function evenArray(arr) {
    arr.forEach(num => {
        if (num % 2 === 0) {
            console.log(num);
        }
    });
}

evenArray(arr);
