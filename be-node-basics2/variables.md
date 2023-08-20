#Lab: JavaScript Variables and Using let and const Instead of var

### Introduction:

In this lab, you will explore JavaScript variables and learn about the differences between the `var`, `let`, and `const` declarations. Understanding these different variable declaration keywords is crucial for writing modern and maintainable JavaScript code.

### Prerequisites:

Node.js installed on your machine.

### Lab Steps:

- Step 1: Create a New Directory:
Create a new directory for your lab work and navigate to it using your terminal or command prompt:

```sh
mkdir variables-node-lab
cd variables-node-lab
```

- Step 2: Create a New JavaScript File:
Create a new file named `variables_lab.js` in the directory.

- Step 3: Open the File in an Editor:
Open the `variables_lab.js` file in your favorite code editor.

- Step 4: Declare Variables Using var:
Inside the `variables_lab.js` file, declare a variable using the var keyword and assign it a value:

```sh
var age = 25;
console.log("Age:", age);
```

- Step 5: Use let for Block-Scoped Variables:
Replace the `var` declaration with  `let` and observe the block-scoping behavior of let:

```js
var age = 25;

if (age > 18) {
    var status = "Adult";
    console.log("Status:", status);
}

// Uncomment the following line to see is 'status' is accessible or not
// console.log("Status outside block:", status);
```

- Step 6: Use `const` for Constants:
Replace the let declaration with const to define a constant variable and try to reassign its value:

```sh
const birthYear = 1998;
// Uncomment the following line to see that reassignment will result in an error
// birthYear = 2000;
console.log("Birth Year:", birthYear);
```

- Step 7: Run the Script:
In your terminal or command prompt, execute the `variables_lab.js` script using the Node.js runtime:

```sh
node variables_lab.js
```

### Conclusion:

You've completed the lab on JavaScript variables and the use of let and const instead of var within a Node.js environment. You've learned about block scoping with let, the immutability of constants with const, and the advantages of using these modern variable declarations for better code maintainability and predictability.

### Optional Further Steps:

- Experiment with variable declarations and assignments in different scenarios to solidify your understanding.
- Explore how variable hoisting works with `var`, `let`, and `const` in Node.js.
- Research how `var`, `let`, and `const` declarations behave when used in functions and modules.




