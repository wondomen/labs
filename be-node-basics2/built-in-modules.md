# Lab: Exploring the OS Built-in Module in Node.js

### Introduction:
In this lab, you will learn how to use the built-in os module in Node.js. The os module provides various functions to interact with the operating system, retrieve system information, and perform system-related tasks.

### Prerequisites:

Node.js installed on your machine.

### Lab Steps:

- Step 1: Create a New Directory:
Create a new directory for your lab work and navigate to it using your terminal or command prompt:

```sh
mkdir os-module-lab
cd os-module-lab
```

Step 2: Create a New JavaScript File:
Create a new file named `os_lab.js` in the directory.

- Step 3: Open the File in an Editor:
Open the `os_lab.js` file in your favorite code editor.

- Step 4: Import and Use the os Module:
Inside the `os_lab.js` file, perform the following steps to use the os module:

**Step 4.1**: Import the os Module:
Import the os module using the require function:

```js
const os = require('os');
```

**Step 4.2**: Use os Module Functions:
Use various functions from the os module to retrieve system-related information. For example:

```js
// Get the platform (e.g., 'win32', 'linux', 'darwin')
const platform = os.platform();
console.log('Platform:', platform);

// Get the operating system's hostname
const hostname = os.hostname();
console.log('Hostname:', hostname);

// Get the architecture (e.g., 'x64', 'arm')
const arch = os.arch();
console.log('Architecture:', arch);

// Get the total system memory in bytes
const totalMemory = os.totalmem();
console.log('Total Memory:', totalMemory, 'bytes');

// Get the free system memory in bytes
const freeMemory = os.freemem();
console.log('Free Memory:', freeMemory, 'bytes');
```

- Step 5: Run the Script:
In your terminal or command prompt, execute the `os_lab.js` script using the Node.js runtime:

```sh
node os_lab.js
```

###  Conclusion:

You've completed the lab on using the os built-in module in Node.js. You've learned how to import the os module, retrieve system information, and perform tasks related to the operating system. The os module is useful for tasks that require system-level information and interactions.

### Optional Further Steps:

- Explore more functions provided by the os module, such as os.cpus(), os.networkInterfaces(), and os.userInfo().
- Experiment with different operating systems to observe how the output of the module's functions varies.
- **Advanced**: Consider combining the information retrieved from the os module with other Node.js modules to create more advanced scripts.




