// JAVASCRIPT CLASS TEST // 

// Section A: Multiple-Choice Questions // 

/*Q1. What will be the output?
● A. null, number, array
● B. object, number, object
● C. object, NaN, array
● D. undefined, number, object*/ 

// console.log(typeof null);
// console.log(typeof NaN);
// console.log(typeof []);

// answer ● B. object, number, object
// explanation: In JavaScript, the typeof operator is used to determine the type of a variable or expression. 
// The typeof operator returns a string indicating the type of the operand. In this case, the first console.log 
// statement will output "object" because obj is an object. The second console.log statement will output "number" 
// because num is a number. The third console.log statement will output "object" because arr is an array, which 
// is also considered an object in JavaScript.

/*Q2. Predict the output.
● A. 205, 200, 24
● B. 205, 200, NaN
● C. NaN, 200, NaN
● D. 2203, 403203, 24*/ 

// console.log(2 + "203");
// console.log(403 - "203");
// console.log(2 * "12abc");

// answer ● none of the above: 2203, 200, NaN
// explanation: In the first console.log statement, the number 2 is concatenated with the string "203", resulting in the string "2203".

/*Q3. Which statement about let, const, and var is correct?
● A. var is block-scoped.
● B. let can be redeclared in the same scope without error.
● C. A const object cannot have its properties modified.
● D. let and const are block-scoped, while var is function-scoped.*/

// answer ● D. let and const are block-scoped, while var is function-scoped.

/*Q4. What is the output?
● A. Pass, Eligible
● B. Pass, followed by a ReferenceError
● C. ReferenceError, ReferenceError
● D. undefined, undefined*/
// let score = 12;
// if (score > 10) {
// var result = "Pass";
// let status = "Eligible";
// }
// console.log(result);
// console.log(status);

// answer ● B. Pass, followed by a ReferenceError
// explanation: The variable result is declared using var, which has function scope. Therefore, it is accessible outside the if block and will output "Pass".

/*Q5. Which loop is most suitable when you need to iterate over the values of an array?
● A. for...in
● B. for...of
● C. if...else
● D. switch*/

// answer ● B. for...of
// explanation: The for...of loop is specifically designed to iterate over the values of iterable objects, such as arrays, strings, and other iterable data structures. It allows you to access each value directly without needing to use an index or key.

/*Q6. What is the main difference between return and console.log() inside a function?
● A. Both return values to the caller.
● B. console.log() returns the calculated result.
● C. return sends a value back to the caller; console.log() displays a value.
● D. return can only be used in arrow functions.*/

// answer ● C. return sends a value back to the caller; console.log() displays a value.
// explanation: The return statement is used to send a value back to the caller of the function, allowing it to be used or stored. On the other hand, console.log() is used for debugging purposes and simply displays a value in the console without returning it to the caller.

/*Q7. What does the rest parameter do in this function?
● A. Converts all arguments into a string.
● B. Collects the arguments into an array.
● C. Expands an existing array into arguments.
● D. Allows only one argument.
function calculateTotal(...prices) {
return prices.length;
}*/

// answer ● B. Collects the arguments into an array.
// explanation: The rest parameter syntax allows a function to accept an indefinite number of arguments as an array. In this case, the ...prices parameter collects all the arguments passed to the calculateTotal function into an array called prices. The function then returns the length of that array, which represents the number of arguments passed.

/*Q8. Which statement about arrow functions and “this” is correct?
● A. Arrow functions always bind this to the object that calls them.
● B. Regular functions always bind this to the object in which they are defined.
● C. Arrow functions inherit this from their surrounding lexical context.
● D. Arrow functions cannot access object properties.*/

// answer ● C. Arrow functions inherit this from their surrounding lexical context.

/*Q9. Operators and type coercion
Predict the output of each statement and explain why the results differ.
console.log("5" + 2);
console.log("5" - 2);
console.log(true + 2);
console.log(Boolean("false"));*/

// + concatenates when one operand is a string.
// - converts strings to numbers.
// true converts to 1.
// Non-empty strings are truthy, including false.

/* Q10. Scope and variable declarations
Write the output in order. Explain why amount and discount behave differently.
var amount = 100;
function calculate() {
var amount = 200;
let discount = 20;
if (true) {
var amount = 300;
let discount = 50;
console.log(amount, discount);
}
console.log(amount, discount);
}
calculate();
console.log(amount);*/

// answer: 300 50, 300 20, 100

/* Q11. Functions and return values
What will be printed? Rewrite the function so that result stores the calculated price.
function calculatePrice(price, quantity) {
console.log(price * quantity);
}
const result = calculatePrice(100, 3);
console.log(result);*/

// answer: 300, undefined

/* Q12. Array mutation
Predict the output. Why are modifications to the array allowed even though it was declared using const?
const products = ["Milk", "Bread", "Rice"];
products[1] = "Eggs";
products.push("Oil");
console.log(products);
console.log(products.length);*/

// answer: ["Milk", "Eggs", "Rice", "Oil"], 4

/* Q13. Object methods and this
Predict the output. What does this refer to during this method call?
const employee = {
name: "Aman",
salary: 30000,
showDetails() {
console.log(this.name, this.salary);
}
};
employee.showDetails();*/

// answer: Aman 30000

/*Q14. Rest parameters and spread syntax
Predict both outputs and explain the difference between the two function calls.
function addNumbers(...numbers) {
return numbers.length;
}
const values = [10, 20, 30, 40];
console.log(addNumbers(values));
console.log(addNumbers(...values));*/

// answer: 1, 4

/* Section C: Debug the Code
Q15. Fix the variable scope issue
The developer wants to print the message after the if block, but the code produces an error. Identify the error,
correct the code, and explain why the original code fails.
if (true) {
let message = "Order placed successfully";
}

console.log(message);*/

// answer: ReferenceError: message is not defined

/*Q16. Fix the shopping cart calculation
Identify the logical error, correct the loop, and explain why the original code produces an incorrect result.
function calculateCartTotal(...prices) {
let total = 0;
for (let i = 0; i <= prices.length; i++) {
total += prices[i];
}
return total;
}
console.log(calculateCartTotal(100, 200, 300));*/

// answer: 600

/* Q17. Fix the object method
Explain why the expected username may not be printed. Rewrite the method correctly and state one situation
where using an arrow function is appropriate.
const user = {
userName: "Rahul",
showName: () => {
console.log(this.userName);
}
};
user.showName();*/

// answer: undefined

/*Q .18 Type Coercion — Predict the Output
console.log([] + []);
console.log([] + {});
console.log("5" - - "2");
console.log(null + 1);
Predict the output of each statement and explain why.*/

// answer: "", "[object Object]", 7, 1

/* Q19. Scope and Hoisting
console.log(a);
var a = 10;

console.log(b);

let b = 20;
● Which statement executes successfully?
● Which statement produces an error?
● Explain the role of hoisting and the Temporal Dead Zone (TDZ).*/

// answer: undefined, ReferenceError: Cannot access 'b' before initialization

/* JavaScript Interview-Level Questions

1. What is the difference between == and ===?*/ 

// answer: The == operator performs type coercion, meaning it converts the operands to the 
// same type before making the comparison. The === operator, on the other hand, checks for 
// both value and type equality without performing any type conversion.

/* 2. What is the difference between undefined and null?
3. What is the difference between for...in and for...of?
4. Can a function return another function? Give a real-world use case.
5. What happens if a function has no explicit return statement?
6. What is the difference between passing a primitive value and passing an object to a function?
7. What is the difference between shallow copying and deep copying an object?
8. Why is NaN !== NaN true?
9. What is the difference between function declarations and function expressions regarding
hoisting?
10. When would you use an arrow function instead of a regular function?*/ 

/* ANSWERS:
// 2. undefined means a variable has been declared but has not yet been assigned a value, while null is an assignment value that represents the intentional absence of any object value.
// 3. for...in iterates over the enumerable properties of an object, while for...of iterates over the values of an iterable object, such as an array or a string.
// 4. Yes, a function can return another function. This is known as a higher-order function. A real-world use case is creating a function that generates customized greeting functions based on the user's name.
// 5. If a function has no explicit return statement, it returns undefined by default.
// 6. When passing a primitive value to a function, a copy of the value is passed, and changes made to the parameter inside the function do not affect the original value. When passing an object, a reference to the object is passed, and changes made to the object's properties inside the function will affect the original object.
// 7. Shallow copying creates a new object with references to the same properties as the original object, while deep copying creates a new object with copies of all nested objects and properties, ensuring that changes to the copied object do not affect the original object.
// 8. NaN !== NaN is true because NaN is not equal to any value, including itself.
// 9. Function declarations are hoisted to the top of their scope, allowing them to be called before they are defined in the code. Function expressions, on the other hand, are not hoisted, and they can only be called after they have been defined.
// 10. Arrow functions are often used for shorter syntax and when you want to preserve the value of this from the surrounding context, such as in callbacks or methods within classes.*/