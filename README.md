# 8th

<!DOCTYPE html> 
<html lang="en"> 
<head> 
<meta charset="UTF-8"> 
<meta name="viewport" content="width=device-width, initial-scale=1.0"> 
<title>JavaScript Conditional Statements</title> 
</head> 
<body> 
<h1>JavaScript Conditional Statements Demo</h1> 
<p>Enter a number:</p> 
<input type="number" id="numberInput"> 
<button onclick="checkNumber()">Check</button> 
<p id="result"></p> 
<script> 
function checkNumber() { 
var number = document.getElementById("numberInput").value; 
if (number > 0) { 
document.getElementById("result").innerHTML = "Number is positive."; 
} else if (number < 0) { 
document.getElementById("result").innerHTML = "Number is negative."; 
} else { 
document.getElementById("result").innerHTML = "Number is zero."; 
} 
switch (true) { 
case (number % 2 === 0): 
document.getElementById("result").innerHTML += " It is even."; 
break; 
case (number % 2 !== 0): 
document.getElementById("result").innerHTML += " It is odd."; 
break; 
default: 
document.getElementById("result").innerHTML += " Invalid input."; 
} 
} 
</script> 
</body> 
</html> 
