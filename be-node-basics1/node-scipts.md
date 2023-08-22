# Lab: Creating and Using Node.js Scripts

### Introduction:

In this lab, you will learn how to create and use Node.js scripts. Node.js allows you to execute JavaScript files as scripts, making it possible to automate tasks, build utilities, and perform various operations using the power of JavaScript.

### Prerequisites:

- Node.js installed on your machine.
- For Windows users, you need also need Git Bash

### Lab Steps:

- Step 1: Create a New Directory:
Create a new directory for your lab work and navigate to it using your terminal or command prompt:

```bash
mkdir node-scripts-lab
cd node-scripts-lab
```

- Step 2: Create a New JavaScript File:
Create a new file named `greeting.js` in the directory. You'll write your script in this file.



- Step 3: Open the File in an Editor:
Open the `greeting.js` file in your favorite code editor.

- Step 4: Write a Regular Function:
Inside the greeting.js file, write a regular function that generates a greeting message using the provided name:

```shell
// greeting.js
function generateGreeting(name) {
  return "Hello, " + name + "!";
}

const personName = "Alice";
const greetingMessage = generateGreeting(personName);
console.log(greetingMessage);
```

- Step 5: Save and Close the File:
Save the changes you made to the greeting.js file.

- Step 6: Run the Script:
Back in your terminal or command prompt, execute the greeting.js script using the Node.js runtime:

```shell
node greeting.js
```

You should see the output: Hello, Alice!.

- Step 7: Modify and Rerun:
Experiment with modifying the personName variable and re-run the script to see how the output changes:

```shell
const personName = "Bob";
const greetingMessage = generateGreeting(personName);
console.log(greetingMessage);
```

### Conclusion:

Congratulations! You've successfully created a Node.js script using regular functions. This lab has shown you how to create a simple script that generates a greeting message using a regular function and runs it using the Node.js runtime.

###  Optional Further Steps:

- Experiment with adding more functions to the script, performing different operations.
- Create a new script file for a different task and practice.





