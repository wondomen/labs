# Lab: Creating and Using Custom Modules

### Introduction:

In this lab, you will learn how to create your own custom modules in Node.js and use them within your scripts. Node.js modules allow you to organize your code into reusable components, promoting modularity and maintainability.

###  Prerequisites:

Node.js installed on your machine.

### Lab Steps:

- Step 1: Create a New Directory:
Create a new directory for your lab work and navigate to it using your terminal or command prompt:

```sh
mkdir custom-modules-lab
cd custom-modules-lab
```

- Step 2: Create Module Files:
Create two new files named `greetings.js` and `app.js` in the directory: `touch greetings.js app.js`
 
- Step 3: Define a Custom Module:
Open the `greetings.js` file in your code editor and define a custom module that exports a function:

```sh
// greetings.js
function greet(name) {
  return "Hello, " + name + "!";
}

module.exports = greet;
```

- Step 4: Use the Custom Module:
Open the `app.js` file and require the custom module you created in the previous step. Use the exported function to generate a greeting message:

```sh
// app.js
const greet = require('./greetings');

const personName = "Alice";
const greetingMessage = greet(personName);
console.log(greetingMessage);
```

- Step 5: Save and Close the Files:
Save the changes you made to both `greetings.js` and `app.js`.

- Step 6: Run the Script:
Execute the `app.js` script using the Node.js runtime:

```sh
node app.js
```

You should see the output: `Hello, Alice!`.

- Step 7: Modify and Rerun:
Experiment with modifying the personName variable in the `app.js` file and re-run the script to see how the output changes:

```sh
const personName = "Bob";
const greetingMessage = greet(personName);
console.log(greetingMessage);
```

### Conclusion:

You've successfully created a custom Node.js module and used it within your script. This lab has shown you how to define and export functions from a module, as well as how to require and use those functions in your application.

### Optional Further Steps:

- Create additional functions in the `greetings.js` module and use them in the `app.js` script.
- Explore different ways to structure your modules, such as exporting multiple functions or exporting an object with properties and methods.
- Experiment with creating multiple modules and organizing them in a directory structure. Use require to load modules from different files and directories.




