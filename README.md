## Var, Let and Const
1. var declarations are globally scoped or function scoped while let and const are block scoped.
1. var variables can be updated and re-declared within its scope; let variables can be updated but not re-declared; const variables can neither be updated nor re-declared.

1.  They are all hoisted to the top of their scope. But while var variables are initialized with undefined, let and const variables are not initialized.

1.  While var and let can be declared without being initialized, const must be initialized during declaration.
<br />
## Filter, Map and Reduce

```
const num = [1, 2, 3];
const newNum = num.map((item) => item * 2);
console.log(newNum);
const sum = newNum.reduce((acc, current) => acc + current, 0);
console.log(sum);
let students = [
  {
    name: "Piyush",
    rollNumber: 31,
    marks: 80
  },
  {
    name: "Jenny",
    rollNumber: 15,
    marks: 69
  },
  {
    name: "kaushal",
    rollNumber: 16,
    marks: 35
  },
  {
    name: "Dilpreet",
    rollNumber: 7,
    marks: 55
  }
];
const totalMarks=students.filter((student)=>student.marks<60).map((item)=> (item.marks+20))
.reduce((acc,current,index,arr)=>
  (acc+current)
,0);
console.log(totalMarks)
```

## Function Declaration
A function declaration also known as a function statement declares a function with a function keyword. The function declaration must have a function name.
Function declaration does not require a variable assignment as they are standalone constructs and they cannot be nested inside a functional block.

```
function geeksforGeeks(paramA, paramB) {
    // Set of statements
}
```
## Function Expressions
A function Expression is similar to a function declaration without the function name.
Function expressions can be stored in a variable assignment.

```
var geeksforGeeks= function(paramA, paramB) {
    // Set of statements
}
```
## IIFE
An IIFE (Immediately Invoked Function Expression) is a JavaScript function that runs as soon as it is defined

```
(function(){
  console.log("This is my immeditely invoked function")
})()
```
