# Lab: npm and VSCode

### Objective: 

In this lab, you'll learn how to utilize npm within Visual Studio Code (VSCode) to manage dependencies, work with scripts, and use the date-fns library for date manipulation in your Node.js projects.

### Prerequisites:

Visual Studio Code installed on your computer.

### Steps

- Step 1: Setting Up Your Project in VSCode
Launch Visual Studio Code.
Create a new directory for your project within VSCode and open it as your workspace.

- Step 2: Managing Dependencies with npm
Open the integrated terminal in VSCode:
Go to the "View" menu and select "Terminal" or press Ctrl + ` (backtick).
Navigate to your project directory using the cd command.
Initialize your project with npm init and follow the prompts.
Install the date-fns library as a project dependency using npm:

```sh
npm install date-fns
```

- Step 3: Working with Scripts
Open your package.json file directly in VSCode.

Locate the "scripts" section and add a script named "start" that runs a sample JavaScript file (e.g., app.js):

```json
"scripts": {
  "start": "node app.js"
}
```

Create a app.js file in your project directory within VSCode and write a simple script that uses date-fns to display the current date and time:

```js
const { format } = require('date-fns');

const currentDate = new Date();
const formattedDate = format(currentDate, 'MMMM d, yyyy');

console.log(`Today's date is ${formattedDate}`);
```

- Step 4: Exploring date-fns in VSCode
In your app.js file, use various functions from the date-fns library to manipulate dates and times.

Run your application using the script you defined earlier within VSCode:

```sh
npm start
```

### Wrapping Up

You've successfully completed this lab, which focused on utilizing npm within Visual Studio Code to manage dependencies, work with scripts, and utilize the date-fns library for date manipulation. Through hands-on experience, you've gained insights into essential tools and practices in Node.js development. As you continue your journey, remember to explore further npm packages, VSCode features, and advanced scripting techniques to enhance your skills.





