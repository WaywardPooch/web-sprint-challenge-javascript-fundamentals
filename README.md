# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge.

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results

### Commits

Set up codegrade early and commit your code regularly and meaningfully.

## Interview Questions

### (please edit this file and write your answer below each question.)

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each.

`.map`, `.reduce`, and `.filter` are all higher order functions used for getting specific information out of arrays.

`.filter` is used when you want to "filter" out specific results, which match a desired criteria, from an array, returning a new filtered array with the information that was picked out.

`.map` likewise returns an array as `.filter` does, but the difference between them is `.map` is used for transforming the filtered information from the array it's looking at to something else (for example, if applied to an array of 'people' objects, you could take the names of each person and where they're from, provided there are keys for each, to return a new array of greeting strings, which use each person's name and location of where they're from, to create dynamic sentences).

Unlike the other two, `.reduce` does not return an array, instead returning a single value, and is used mainly for performing calculations from elements in an array.

1. Explain the difference between a callback and a higher order function.

   - A **callback function** is a function that is fed _into_ a **higher order function** as an argument to take the place of that higher order function's callback parameter.

2. Explain what a closure is.

   - **Lexical scope** is the idea that _nested_ functions have access to the variables and functions of scopes _outside_ of their immediate local scope (and the functions and variables on the _outside_ can't access the variables and functions _inside_ of their nested functions). **Closure** is the fact that, in addition to this idea of **lexical scope**, nested functions have access to the information of their parents _even after_ the parent functions have closed.

3. Describe the four principles of the 'this' keyword.

   1. **Window binding** is when `this` is not given proper context and has no other choice but to "guess" what the developer meant by binding itself to the global javaScript object; this is generally an error, _not_ behavior that most developers intend.
   2. **Implicit binding** is when the context of `this` is _implied_ as being the object to the left of the `.` operator when methods of objects that require `this` are invoked.
   3. **Explicit binding** is when the context of `this` is _explicitly_ set through the invocation of functions using either the `.apply()`, `.bind()`, or `.call()` methods, with the object to take the place of `this` passed in as an argument to one of these methods.
   4. **New binding** is when the context of `this` is set to the object made during the creation of a new object from an object constructor function, invoked using the `new` operator before it.

4. Why do we need super() in an extended class?

   - Without invoking `super()` inside of an extended class, the extended class will _not_ inherit the properties and methods of its parent class. You also need to pass in the attributes shared between the parent and child classes as an argument for `super()` for this functionality to work as-intended.

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade.

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:

1. Fork the repo
2. Clone your forked version of the repo
3. cd into your repo and create a branch with your first and last name
4. open the terminal in your vs code and type `npm install`
5. next type `npm run test` in your terminal
6. Complete your work making regular commits, once you have all your tests passing and you are ready to submit your work please see canvas for instructions on how to submit

### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start`
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources

[Sprint Challenge Study Guide](https://www.notion.so/lambdaschool/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://www.notion.so/lambdaschool/Submitting-an-assignment-via-Code-Grade-A-Step-by-Step-Walkthrough-07bd65f5f8364e709ecb5064735ce374)
