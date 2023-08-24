# Lab: Creating a React Project and Understanding Dependencies

In this lab, you'll create a new React project and explore its dependencies, including dev dependencies. You'll also understand why `import` is used instead of `require` in modern React projects.

**Step 1: Setting Up Your Environment**

1. **Create a New React App:**
   Open your terminal and run:
   
```sh
npx create-react-app react-dependencies-lab
cd react-dependencies-lab
```

**Step 2: Exploring Project Dependencies and Dev Dependencies**

1. **Open `package.json`:**
   Open the `package.json` file located in your project's root directory. This file lists the dependencies and dev dependencies of your project.

2. **Project Dependencies:**
   Look for the `"dependencies"` section in `package.json`. These are the packages required for your app to run properly. Some common dependencies might include `react` and `react-dom`. You can install these packages using `npm install`.

   Hints: 
   - Look for lines like `"react": "^18.2.0"` and `"react-dom": "^18.2.0"` under `"dependencies"`.

3. **Dev Dependencies:**
   Dev dependencies are packages required during development, but not in production. They include tools for testing, code linting, bundling, etc. They should be listed under the `"devDependencies"` section.

   - Do you see `"devDependencies"` section in `package.json`. 

   Hint: Check this [thread]


**Step 3: Understanding `import` vs. `require`**

1. **`import` vs. `require` in Modern React:**

   In modern React projects, including those created with Create React App, the preferred way to import modules is using the `import` statement. This is because `import` is part of the ES6 module syntax, which offers various benefits:

   - `import` supports named imports and default imports.
   - `import` allows for tree shaking, which optimizes unused code during the build.
   - `import` is statically analyzable, aiding tooling and optimizations.

   **Why `import` Over `require`:**

   React projects are set up to use ES6 modules and the `import` syntax. While `require` is common in Node.js (CommonJS), using `require` in modern React projects could lead to compatibility issues and errors.

**Summary:**

In this lab, you created a new React project and explored its dependencies, including project dependencies and dev dependencies. You learned the distinction between them and how to identify them in the `package.json` file. Additionally, you understood why the `import` statement is favored over `require` in modern React projects, thanks to its compatibility with ES6 modules and its advantages in terms of code optimization and tooling.

<!-- Links -->

[thread]:https://stackoverflow.com/questions/44868453/create-react-app