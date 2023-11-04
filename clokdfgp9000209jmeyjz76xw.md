---
title: "Basic JavaScript Concepts."
seoTitle: "Mastering the Fundamentals: A Comprehensive Guide to Basic JavaScript"
seoDescription: "Mastering the Fundamentals: A Comprehensive Guide to Basic JavaScript"
datePublished: Sat Nov 04 2023 18:21:42 GMT+0000 (Coordinated Universal Time)
cuid: clokdfgp9000209jmeyjz76xw
slug: basic-javascript-concepts
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1699121138526/48d22cf6-1ac9-4e6e-bcc0-904e6de1c825.gif
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1699122055283/49aff371-e93b-4b58-9670-6d3b8decd2df.png
tags: js, javascript, web-development, frontend-development

---

## What is the difference between words and Keywords in JavaScript?

#### Word.

Anything that doesn't have a particular meaning in JavaScript is called a word.

```plaintext
For example.
my_Name, my_Age, my_Gender, num, x, y, z, a, b ,c

They all are words 👆 
```

#### Keyword.

Keywords in JavaScript are words with assigned tasks and have some meanings.

```javascript
// For example
let
const
if 
else if
while
break
this
async

// They all are keywords as they have some meaning in JavaScripy.
```

## What are variables & constants in JS?

#### What are variables?

The variable is something that changes.

#### Variables in programming?

In programming, if you want to store some data or information then you need variables that help you to store your data or information. You can change their values and update them as well.

#### Types of Variables in JS.

In JavaScript, you can declare or initialize variables in two ways.

1. let
    
2. var
    

#### What are constants in JS?

The constant is something that never changes.

#### Constant in JS?

In JavaScript, you can declare constant in only one way that is with const. You can never update const values and you can't redeclare them.

## What is Undefined & Not defined?

Let's understand this with the help of an example.

#### Undefined.

If you have a variable in JS that you have declared but you didn't assign it a value. Then you console.log it and an error appears called the value of your variable is undefined. That means that JS finds your variable but doesn't find any value assigned to it.

```javascript
// for exmaple

let my_Name;
console.log(my_Name); //undefined
```

#### Not defined.

Assuming you haven't declared and initialized the my\_Age variable, attempting to log it will result in a not-defined error.

```javascript
// for example
console.log(my_Age); // notdefined
```

## Hoisting in JavaScript?

Hoisting in JavaScript is a behavior where variable and function declarations are moved to the top of their containing scope during the compile phase before the code is actually executed. This means that you can use a variable or a function before it has been declared.

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">However, it's important to note that only the declarations are hoisted, not the initializations. This means that while you can use a variable or function before it's formally declared, the value assigned to the variable or the function definition won't be available until after the declaration.</div>
</div>

```javascript
console.log(myVariable); // Output: undefined
var myVariable = 10;
```

In the above code, `myVariable` is hoisted to the top of its scope, but its value is not yet defined. So, when you try to `console.log(myVariable)`, it prints `undefined`.

Similarly, with functions.

```javascript
myFunction(); // Output: "Hello!"
function myFunction() {
    console.log("Hello!");
}
```

In this case, `myFunction` is hoisted to the top of its scope, so you can call it before its actual declaration in the code.

## Data types in JS?

In JavaScript, there are two types of data.

1. Primitive data types.
    
2. Reference data types.
    

#### Primitive Data Types.

In the primitive data type, we have the following data types.

1. String
    
2. Number
    
3. Boolean
    
4. Undefined
    
5. Null
    
6. BigInt (ES11)
    
7. Symbol (ES6)
    

#### Reference Data Types.

In the reference data type, we have the following data types.

1. Functions
    
2. Arrays
    
3. Objects
    
4. Class (ES6)
    

## Loops in JS?

In JavaScript, loops are control structures that allow you to repeatedly execute a block of code as long as a specified condition is true.

There are different types of loops in JS, but on the basis of JavaScirpt, we will talk about for loop and while loop.

#### for loop.

for loop consists of three parts.

1. The starting point of the loop.
    
2. The endpoint.
    
3. The interaction you want to make.
    

```javascript
// for example
for(let i = 1; i <= 10; i++){
    console.log(i*2)
}

// output : table of 2 printed.
```

#### While loop.

While loop also consists of three parts same as for the loop but their order is different

```javascript
// for example

/* 

starting point;
while(condition the must be false in future){
        // print the value
The change you want to made.
}

*/

let a = 1;
while(a <= 10){
    console.log(a*3);
    a++;
}

// output : table of three printed
```

## Functions in JS?

A function is mainly used for three things.

1. If you want to reuse your code.
    
2. If you want your code to run later in the future when you need it.
    
3. if you want to run your code with new inputs every time.
    

#### Parameters in function.

Variables that store the value of arguments are called parameters.

#### Arguments in function.

Arguments in function are nothing but real value that you have passed every time you call the function.

![What are Argument and Parameter in Javascript with examples | by Chitru  Shrestha | Medium](https://miro.medium.com/v2/resize:fit:884/1*VREE2YzaGUUSBVhHTHo4HA.png align="right")

#### In how many ways we can write functions in JS?

There are six styles in which we can write our functions in JS. Three styles come in ES6 and three come in ES6 versions.

1. Function Declaration
    
2. Function Expression
    
3. Arrow Function(ES6)
    
4. Arrow Function with Implicit Return (ES6)
    
5. Immediately Invoked Function Expression (IIFE)
    
6. Function inside an object
    

#### Let's create a simple function in JS.

```javascript
// Lets do this with function decleration first.
function std_Details(name, age, profession){
    return `name: ${name}, age: ${age}, profession: ${profession}`;
}

console.log(std_Details("Muhammad Shakir",22,"Front-end Dev"));

// lets do this funciton expression
let std_Details = funciton(name,age,depart){
    return `name: ${name}, age: ${age}, depart: ${depart}`;
}

console.log(std_Details("Muhammad Haris",22,"Software Engineering"));

// let do this with arrow funciton : My Favorite😁
let std_Details = (name, email, std_ID) => {
    return  `name: ${name}, email: ${email}, std_ID: ${std_ID}`;
}

console.log(std_Details("Muhammad Shakir","xyz@gmail.com",77));
```

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">In the basic, we will only cover these three styles</div>
</div>

## Arrays in JS?

An array is a type of Data Structure, that stores multiple values of multiple data types. You can also call it a group of values. Array use index numbers to store values and index number starts from 0 to nth. An index is a counting to the array.

```javascript
// for example
let ary = ['Muhammad Shakir',22,'xyz@gmail.com'];
console.log(ary[0]); // Muhammad Shakir
console.log(ary[1]); // 22
console.log(ary[2]); // xyz@gmail.com
```

## Objects in JS?

Let’s understand it with an example.

1. If you want to store multiple data of multiple persons let’s say names of different persons then here you can use array.
    
2. But if you want to store multiple data of a single person in a key-value pair then here you can use Objects.
    

#### Types of Objects.

1. Blank Objects.
    
2. Filled Objects.
    

```javascript
// for example
let subDetails = {
    name: 'Software Engineering',
    code: 'SE-101',
    creditHours: 3.5
}

// lets print the value of array.
console.log(subDetails.name); // Software Engineering
console.log(subDetails.code); // SE-101
console.log(subDetails.creditHours); // 3.5
```

## Methods in JS?

A property in an object whose value is a function is called a method.

```javascript
// lets create a calculator obj and inside it's diff methods.

let calculator = {
    sum(x,y){
        return x + y
    },

    sub(x,y){
        return x - y
    }
}

// for accessing the methods.
console.log(calculator.sum(4 , 5)); // 9
console.log(calculator.sub(5 , 4)); // 1
```