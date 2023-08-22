# Lab: Refactoring Regular Functions to Arrow Functions

### Introduction:

In this lab, you will explore various scenarios where you can **refactor** regular functions into arrow functions in JavaScript. Arrow functions provide a concise syntax and lexically scoped this, making them a valuable tool for enhancing code readability and maintainability.

### Prerequisites:

Node.js installed on your machine.

### Lab Steps:

- Step 1: Create a New Directory:
Create a new directory for your lab work and navigate to it using your terminal or command prompt:

```shell
mkdir arrow-function-lab
cd arrow-function-lab
```

- Step 2: Create a New JavaScript File:
Create a new file named `refactor_lab.js` in the directory.
  - On Linux/macOS: `touch refactor_lab.js`
  - On Windows:`notepad refactor_lab.js`


- Step 3: Open the File in an Editor:
Open the refactor_lab.js file in your favorite code editor.

- Step 4: Refactor Regular Functions to Arrow Functions:
Inside the `refactor_lab.js` file, perform the following refactoring from regular functions to arrow functions:

**Scenario 1**: Basic Function:
Refactor a simple function with no parameters and a single-line return statement:

```js
// Regular function
function sayHello() {
    return "Hello, world!";
}
```

<details>
  <summary>Solution</summary>

const sayHelloArrow = () => "Hello, world!";

</details>


**Scenario 2**: Single Parameter:
Refactor a function with a single parameter:

```js
// Regular function
function double(x) {
    return x * 2;
}
```

<details>
  <summary>Solution</summary>

const doubleArrow = x => x * 2;

</details>


**Scenario 3**: Multiple Parameters:
Refactor a function with multiple parameters:

```js
// Regular function
function add(x, y) {
    return x + y;
}
```

<details>
  <summary>Solution</summary>

const addArrow = (x, y) => x + y;

</details>

**Scenario 4**: Function Inside an Object:
Refactor a function defined inside an object:

```js
// Regular function
const person = {
    name: "Alice",
    sayHi: function() {
        return "Hi, " + this.name + "!";
    }
};
```

<details>
  <summary>Solution</summary>
<pre>
const personArrow = {
    name: "Alice",
    sayHi: () => "Hi, " + this.name + "!" // 'this' will not work as expected here
};
</pre>
</details> 


**Scenario 5**: Callback Functions:
> Call back functions and map() will be discussed later in the course

Refactor a callback function passed to the map method:

```js
const numbers = [1, 2, 3, 4, 5];

// Regular function
const doubled = numbers.map(function(num) {
    return num * 2;
});
```

<details>
  <summary>Solution</summary>

const doubledArrow = numbers.map(num => num * 2);

</details>

- Step 5: Run the Script:
In your terminal or command prompt, execute the `refactor_lab.js` script using the Node.js runtime:

```shell
node refactor_lab.js
```

### Conclusion:

You've completed the lab on refactoring regular functions to arrow functions in various scenarios. You've learned how arrow functions provide a more concise and expressive syntax for writing functions, making your code cleaner and more maintainable.

### Optional Further Steps:

- Explore other scenarios where you can refactor regular functions to arrow functions.




