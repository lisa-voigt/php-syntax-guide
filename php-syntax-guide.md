# Lisa's PHP Syntax Guide

### Welcome to my PHP syntax guide, where coding meets canine charm in the third installment of syntax brilliance, dedicated to the one and only, Lola!

## Comments 

Comments in PHP are essential for adding notes and explanations to your code. They are not executed and serve as helpful documentation for yourself and others.

```
<?php
// This is a single-line comment - Lola is my dog. 

/*
   This is a multi-line comment
   useful for longer explanations or disclaimers for when I need more than
   one line to gush about how great my dog is. 
*/
?>
```

## Variables

Variables in PHP are containers for storing information and can hold various data types.

```
<?php
$dogName = "Lola";
$age = 11;
$isSoSweet = true;
?>
```

## Echo/Print

Echo and print are used to output data. Echo is faster and can take multiple parameters. Print can only handle one paramter and returns a value.

```
<?php
$phrase = "Lola, my loyal companion.";

echo $phrase; // Outputs: Lola, my loyal companion.

print "Shepherd Husky cross: " . $phrase; // Outputs: Shepherd Husky cross: Lola, my loyal companion.
?>
```

## Data Types

PHP supports various data types, including strings, integers, floats, booleans, arrays, and more.

```
<?php
$greeting = "Hello"; // String
$age = 11; // Integer
$weight = 59.5; // Float
$isSenior = true; // Boolean
?>
```

## Strings

Strings in PHP are sequences of characters. They can be declared using single or double quotes.

```
<?php
$dogBreed = 'Shepherd Husky Cross'; // Using single quotes
$dogColor = "Black and Tan"; // Using double quotes
?>
```

## Numbers 

Numbers in PHP can be integers or floats.
An integer is a whole number without any decimal point. A float is a number that has a decimal point or is expressed in scientific notation.

```
<?php
$yearsOld = 11; // Integer
$weight = 30.5; // Float
?>
```

## Constants

Constants are like variables but cannot be changed once defined. They are often used for values that remain the same throughout the script.

```
<?php
define("MAX_WEIGHT", 59);
echo MAX_WEIGHT; // Outputs: 59
?>
```

## Operators 

Operators in PHP are used for performing operations on variables and values.

```
<?php
$number1 = 10;
$number2 = 5;

$sum = $number1 + $number2; // Addition
$product = $number1 * $number2; // Multiplication
?>
```

## If & Else & Elseif

Conditional statements in PHP are used for decision-making in code execution. Conditional statements allow the code to decide what message to display based on the temperature. The conditions are evaluated in order, and the first true condition determines which block of code gets executed.

```<?php
$temperature = 25;

if ($temperature > 30) { // this statement is false because the temperature is < 30 so the elseif statement will be evaluated. 
    echo "It's too hot outside for Lola!"; 
} elseif ($temperature > 10) { 
    echo "This is great weather for Lola."; // this is the message that will be displayed (echoed) because the temperature is > 10 but also < 30. 
} else {
    echo "This is Lola's ideal temperature, she is a Husky after all!"; // this statement didn't get evaluated because the previous one was true. 
}
?>
```

## Functions

A function in PHP is a named block of code that can be defined once and called multiple times within a script. Functions help organize and modularize code by allowing you to encapsulate a set of instructions into a single unit.

```
function functionName($parameter1, $parameter2, ...) {
    // Code to be executed
    // ...
    return $result; // Optional: Functions can return a value
}

<?php
$name = "Lola";

function greet($name) {
    echo "Hello, $name!";
}

greet("Lola"); // Outputs: Hello, Lola!
?>
```

## Arrays

Arrays in PHP store multiple values in a single variable.

```
<?php
$favoriteTreats = array("Salmon", "Bacon", "Cheese");

echo "Lola's favorite treat is the " . $favoriteTreats[0] . ".";
// Outputs: Lola's favorite treat is Salmon.
?>
```

## Loops 

Loops in PHP allow you to execute a block of code repeatedly. Here's an example of a PHP loop in the context of Lola's training to learn new tricks. 

```
<?php
$tricksToLearn = array("Sit", "Stay", "Roll Over", "Fetch", "High Five");

echo "Lola's Trick Training Sessions:<br>";

foreach ($tricksToLearn as $index => $trick) {
    $sessionNumber = $index + 1;
    echo "Session $sessionNumber: Teach Lola to $trick<br>";
}
?>
```