# Assignment-5
1. The Document Object Model, Predefined objects, Object-oriented language, HTML Element, Variables, Scope , Operators, Functions, Conditional statements, Looping statements

-->Document Object Model (DOM): The DOM represents the structure of an HTML document as a tree of objects. Each element becomes a node in this tree, and JavaScript can use it to manipulate HTML dynamically.
\\Example code:
  <p id="demo">Hello</p>
  <script>
    document.getElementById("demo").innerHTML = "Hello, DOM!";
  </script>
-->Predefined Objects:
JavaScript comes with several built-in objects like:
  Math → for mathematical operations
  Date → for handling dates
  Array, String, Object → for working with data structures
\\Example code:
  let x = Math.sqrt(25);  // 5
  let today = new Date(); // current date
-->Object-Oriented Language: JavaScript supports object-oriented programming (OOP), meaning we can create and use objects with properties and methods.
\\Example code:
  let person = {
    name: "Alice",
    age: 25,
    greet: function() {
      return "Hello, " + this.name;
    }
  };
-->HTML Element: An HTML element is any part of an HTML document like <p>, <div>, <img>, etc.
\\Example code:
  <button onclick="alert('Hello')">Click Me</button>
-->Variables and Scope: Variables store data. Scope defines where the variable can be accessed.
-->Operators: 
Used to perform operations:
  Arithmetic: +, -, *, /
  Comparison: ==, ===, !=, <, >
  Logical: &&, ||, !
-->Functions: Reusable blocks of code.
\\Example Code:
  function greet(name) {
    return "Hello, " + name;
  }
-->Conditional Statements: Decide what to do based on conditions.
\\Example code:
  if (age > 18) {
    alert("Adult");
  } else {
    alert("Minor");
  }
-->Looping Statements: Repeat a block of code.
\\Example code:
  for (let i = 0; i < 5; i++) {
    console.log(i);
  }
  
  let i = 0;
  while (i < 5) {
    console.log(i);
    i++;
  }

2. Understand the data types, understand the difference between Let, Var and const with example, understand the scope of these variables.
-->Data types in JavaScript:
    String: "hello"
    Number: 42
    Boolean: true/false
    Array: [1, 2, 3]
    Object: { name: "John" }
    undefined, null

-->let vs var vs const
    function test() {
      if (true) {
        var x = 10;
        let y = 20;
        const z = 30;
      }
      console.log(x); // 10 (function scoped)
      // console.log(y); ❌ Error (block scoped)
      // console.log(z); ❌ Error (block scoped)
    }

