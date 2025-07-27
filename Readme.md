Subject:

A variable points to a specific memory address that stores a value. 
Variables are given a name which can be used throughout your code to access that value.

Declaring a variable means giving it a name. 
In JavaScript, this is often done with the let keyword. 
**Example Code:**
```
    let hello;
```
Variable naming follows specific rules: 
names can include letters, numbers, dollar signs, and underscores, 
but cannot contain spaces and must not begin with a number.

Assigning a value to a variable at the moment of its declaration is known as initialization.


JavaScript has seven primitive data types, with **String** being one of them. 
In JavaScript, a string represents a sequence of characters and can be enclosed in either single (') or double (") quotes.

Note that strings are **immutable**, which means once they are created, they cannot be changed. The variable can still be reassigned another value.


The console allows you to print and view JavaScript output. 
You can send information to the console using console.log(). 
**Example Code:**
```
    let developer = "Naomi";
    console.log(developer);
```


When a variable is declared with the **let** keyword, you can reassign (or change the value of) that variable later on. 
**Example Code:**
```
    let programmer = "Naomi";
    programmer = "CamperChan";
```
Note that when reassigning a variable, you do not use the let keyword again.


When variable names are more than one word, there are specific naming conventions for how you capitalize the words. 
In JavaScript, the convention to use is **camel case**.

Camel case means that the first word in the name is entirely lowercase, but the following words are all title-cased. 
**Example Code:**
```
    let variableOne;
    let secondVariable;
    let yetAnotherVariable;
    let thisIsAnAbsurdlyLongName;
```


When you declare a variable without initializing it, it is considered **uninitialized**. 

The default value of an uninitialized variable is undefined. 
This is a special data type that represents a value that does not have a definition yet.

You can still assign a value to an uninitialized variable.
**Example Code:**
```
    let uninitialized;
    uninitialized = "assigned";
```


With the **number data type**, you can perform mathematical operations, like addition. 


An array is a non-primitive data type that can hold a series of values. 
Non-primitive data types differ from primitive data types in that they can hold more complex data. 
Primitive data types like strings and numbers can only hold one value at a time.

Arrays are denoted using square brackets ([]). 
**Example Code:**
```
    let array = [];
```

When an array holds values, or **elements**, those values are separated by commas. 


You can access the values inside an array using the index of the value. 
An index is a number representing the position of the value in the array, starting from 0 for the first value.

You can access the value using bracket notation, such as array[0].


Arrays are special in that they are considered **mutable**. 
This means you can change the value at an index directly.


A **method** in JavaScript is a function that's associated with certain values or objects. 
An example you've already encountered is the .log() method, which is part of the console object.


Arrays have their own methods, and the first you will explore is the **.push()** method. 
This allows you to "push" a value to the end of an array.


Another method essential for this project is the **.pop()** method. 
It removes the last element from an array and returns that element.


A const variable cannot be reassigned like a let variable. 
This code would throw an error:
**Example Code:**
```
    const firstName = "Naomi";
    firstName = "Jessica";
```

A const variable also cannot be uninitialized. 
This code would throw an error:
**Example Code:**
```
    const firstName;
```


When you have to perform a task repeatedly until a condition is met, you will use a loop. 
There are many ways to write a loop.

You are going to start with a basic for loop. 
for loops use the following syntax:
**Example Code:**
```
    for (iterator; condition; iteration) {
    logic;
    }
```

The **iterator** is a variable you can declare specifically in your for loop to control how the loop iterates or goes through your logic.
**Example Code:**
```
    for (let index = 100; "second"; "third") {
    }
```


The **condition** of a for loop tells the loop how many times it should iterate. 
When the condition becomes false, the loop will stop.

In JavaScript, a Boolean value can be either true or false


for...of loop, which iterates over each item in an iterable object and temporarily assigns it to a variable.

The syntax for a for...of loop looks like:
Example Code:
```
    for (const value of iterable) {

    }
```
Note that you can use const because the variable only exists for a single iteration, not during the entire loop.


**escape sequence** \n, which is interpreted as a new line when the string is logged.
Example Code:
```
    lineOne = lineOne + "\n" + lineTwo;
```


.repeat() method available to strings. 
This method accepts a number as an argument, specifying the number of times to repeat the target string. 
For example, using .repeat() to generate the string "Code! Code! Code!":

Example Code:
```
    const activity = "Code! ";
    activity.repeat(3);
```


A function is a block of code that can be reused throughout your application. 
Functions are declared with the following syntax:
Example Code
```
    function name(parameter) {

    }
```
The function keyword tells JavaScript that the name variable is going to be a function. 
parameter is a variable that represents a value that is passed into the function when it is used. 
A function may have as many, or as few, parameters as you'd like.


When you have a value that is explicitly written in your code, like the "Hello!" string in your function, it is considered to be **hard-coded**.
Hard-coding a value inside a function might not make it as reusable as you'd like.

Instead, you can define **parameters** for the function. 
Parameters are special variables that are given a value when you call the function, and can be used in your function to dynamically change the result of the function's code.


Variables in JavaScript are available in a specific scope. 
In other words, where a variable is declared determines where in your code it can be used.

The first scope is the **global scope**. 
Variables that are declared outside of any "block" like a function or for loop are in the global scope. 
Your character, count, and rows variables are all in the global scope.

When a variable is in the global scope, a function can access it in its definition.


Variables can also be declared inside a function. 
These variables are considered to be in the **local scope**, or **block scope**. 
A variable declared inside a function can only be used inside that function. 
If you try to access it outside of the function, you get a reference error.


An important thing to know about the return keyword is that it does not just define a value to be returned from your function, it also stops the execution of your code inside a function or a block statement. 
This means any code after a return statement will not run.


A function call allows you to actually use a function. 
You may not have been aware of it, but the methods like .push() that you have been using have been function calls.


The values you provide to a function call are referred to as arguments, and you pass arguments to a function call.


Remember that you can use the + operator to concatenate strings like this:
Example Code:
```
    " " + "string"
```


The **addition operator** is not the only way to add values to a variable. 
The **addition assignment operator** can be used as shorthand to mean "take the original value of the variable, add this value, and assign the result back to the variable." 
Example Code:
```
    test = test + 1;
    test += 1;
```


Comments can be helpful for explaining why your code takes a certain approach, or leaving to-do notes for your future self.
In JavaScript, you can use // to leave a single-line comment in your code.


JavaScript also has support for multi-line comments. 
A multi-line comment starts with /* and ends with */.
Unlike a single-line comment, a multi-line comment will encapsulate multiple lines.


An if statement allows you to run a block of code only when a condition is met. 
They use the following syntax:
Example Code:
```
    if (condition) {
    logic
    }
```


A truthy value is a value that is considered true when evaluated as a boolean. 
Most of the values you encounter in JavaScript will be truthy.

A falsy value is the opposite - a value considered false when evaluated as a boolean. 
JavaScript has a defined list of falsy values. 
Some of them include **false**, **0**, **""**, **null**, **undefined**, and **NaN**.


In addition to if statements, JavaScript also has else if statements. 
else if statements allow you to check multiple conditions in a single block of code.


A while loop will run over and over again until the condition specified is no longer true. 
It has the following syntax:
Example Code:
```
    while (condition) {
    logic;
    }
```


The **equality operator** == is used to check if two values are equal.


The **strict equality operator** === is used to check if two values are equal and share the same type. 
As a general rule, this is the equality operator you should always use.


The **strict inequality** operator !== allows you to check if two values are not equal, or do not have the same type. 
The syntax is similar to the equality operator: value !== 4.


The **subtraction assignment operator** -= subtracts the given value from the current variable value, then assigns the result back to the variable.


The .unshift() method of an array allows you to add a value to the beginning of the array, unlike .push() which adds the value at the end of the array. 
.unshift() returns the new length of the array it was called on.
Example Code:
```
    const countDown = [2, 1, 0];
    const newLength = countDown.unshift(3);
    console.log(countDown); // [3, 2, 1, 0]
    console.log(newLength); // 4
```


ternary operator: condition ? exprIfTrue : exprIfFalse

arrow function: const var = () => { }


loop (code alternative)
    for (let i = 1; i <= count; i++) {
    rows.push(padRow(i, count));
    }
    while (rows.length < count) {
    rows.push(padRow(rows.length + 1, count));
    }
    for (let i = count; i > 0; i--) {
    rows.push(padRow(i, count));
    }

