# Lab: Exploring npm: 

## Part 1/3

### Introduction:
In this lab, you will learn how to use the date-fns library for date manipulation and formatting in JavaScript. Additionally, you'll gain an understanding of the node_modules directory, which stores the packages you install using npm.

### Prerequisites:

Node.js and npm installed on your machine.

### Lab Steps:

- Step 1: Create a New Project:

Create a new directory for your lab work and navigate to it using your terminal:

```sh
mkdir date-fns-lab
cd date-fns-lab
```

Initialize a new Node.js project:

```sh
npm init -y
```

- Step 2: Install date-fns:

Install the date-fns library as a dependency using npm:

```sh
npm install date-fns
```

- Step 3: Explore the node_modules Directory:

After installing date-fns, you'll notice a new directory called node_modules in your project folder. This directory stores all the packages you install using npm.

Open the node_modules directory to see the subdirectories and files that correspond to the installed packages. Each package has its own folder within node_modules.

- Step 4: Create a Date Manipulation Script:

Create a file named dateManipulation.js in your project directory.

Import the necessary functions from the date-fns library:

```sh
const { addDays, format } = require('date-fns');
```

Create a JavaScript function that demonstrates date manipulation using date-fns:

```sh
function manipulateDate() {
  const currentDate = new Date();
  const futureDate = addDays(currentDate, 7);
  
  console.log('Current Date:', format(currentDate, 'MMMM dd, yyyy'));
  console.log('Date 7 days from now:', format(futureDate, 'MMMM dd, yyyy'));
}

manipulateDate();
```

- Step 5: Run the Script:
Run the dateManipulation.js script using the Node.js runtime:

```sh
node dateManipulation.js
```

###  Conclusion:

You've completed the lab on using the date-fns library for date manipulation and formatting. You've also gained an understanding of the node_modules directory, which holds the packages installed using npm. This directory is crucial for managing dependencies in your Node.js projects.

### Optional Further Steps:

- Explore more functions provided by date-fns and experiment with different date manipulation scenarios.
- Experiment with installing additional packages and observe how they are added to the node_modules directory.


----

## Part 2/3

### Introduction:

In this lab, you will learn how to use npm (Node Package Manager) to manage dependencies, initialize projects, run scripts, and more. npm is a powerful tool that allows you to easily manage packages and streamline your development workflow.

### Prerequisites:

Node.js and npm installed on your machine.

Lab Steps:

- Step 1: Initialize a New Project:

Create a new directory for your lab work and navigate to it in your terminal:

```sh
mkdir npm-lab
cd npm-lab
```

Initialize a new Node.js project using the following command. This will create a `package.json` file that tracks your project's dependencies and settings:

```sh
npm init -y
```

- Step 2: Install Dependencies:

Install a package as a dependency. For this lab, let's install the popular lodash library as an example:

```sh
npm install lodash
```

Check the package.json file to see that lodash has been added as a dependency.

- Step 3: Install Dev Dependencies:

Install a package as a dev dependency. For instance, let's install jest for testing:

```sh
npm install jest --save-dev
```

Observe the changes in the package.json file under the "devDependencies" section.

- Step 4: Create and Run Scripts:

Open the package.json file and locate the "scripts" section. This is where you can define custom scripts to run tasks.

Add a new script to the "scripts" section to run tests using jest:

```json
"scripts": {
  "test": "jest"
}
```

Save the package.json file.

Run the script you defined using the following command:

```sh
npm test
```

- Step 5: Explore package.json:

Open the package.json file and explore its contents. You'll find information about the project, its dependencies, dev dependencies, scripts, and more.

- Step 6: Uninstall Packages:

If needed, you can uninstall a package using the npm uninstall command. For example, let's uninstall lodash:

```sh
npm uninstall lodash
```

Observe that the package.json file no longer lists lodash as a dependency.

### Conclusion:
Congratulations! You've completed the lab on using npm to manage dependencies, initialize projects, run scripts, and more. npm is a versatile tool that greatly simplifies the management of packages and helps streamline your development process.



----
## Part 3/3

### Introduction:
In this extended lab, you will continue building upon the previous lab by adding a unit test using Jest and learning how to use the lodash library. You'll explore how to write a simple test, run it using npm scripts, and utilize lodash for common utility functions.

### Prerequisites:

Node.js and npm installed on your machine.

### Lab Steps:

- Step 1: Initialize a New Project:

Follow the initialization steps from the previous lab to set up your project.

- Step 2: Install Dependencies and Dev Dependencies:

Follow the steps from the previous lab to install the lodash library as a dependency and jest as a dev dependency.

- Step 3: Create a Simple JavaScript Function:

Create a file named math.js in your project directory.

Define a simple math function in math.js that adds two numbers:

```js
function add(a, b) {
  return a + b;
}

module.exports = add;
```

- Step 4: Write a Unit Test Using Jest:

Create a file named math.test.js in your project directory.

Write a simple test for the add function using Jest:

```js
const add = require('./math');

test('adds 1 + 2 to equal 3', () => {
  expect(add(1, 2)).toBe(3);
});
```


- Step 5: Update package.json Scripts:

Open the package.json file and add the following script to the "scripts" section to run tests using Jest:
```json
"scripts": {
  "test": "jest"
}
```

- Step 6: Use lodash in Your Code:

Open the math.js file again.

Import the lodash library at the top of the file:

```js
const _ = require('lodash');
```

Use lodash's utility functions in your add function:

```js
function add(a, b) {
  return _.add(a, b);
}

module.exports = add;
```

- Step 7: Run the Unit Test:

Run the test you wrote using the following command:
```sh
npm test
```

### Conclusion:

You've completed the extended lab on using npm to manage dependencies, scripts, and unit tests. You've also learned how to use the lodash library for utility functions. This lab has provided you with practical experience in setting up tests and using external libraries to enhance your code.

### Optional Further Steps:

- Experiment with creating additional scripts in the "scripts" section of the package.json file.
- Explore how to install packages globally using the -g flag.
- Research and use other npm commands like npm update, npm outdated, and npm search to manage packages effectively.

