# Lab: Creating Your First React Component**

In this lab, we'll create a simple React component to display information using JSX. We'll cover JSX syntax, importing/exporting components, JSX vs. HTML, and how to render JSX content.

### Step 1: Setting Up Your Environment

Before you start, ensure you have Node.js and npm (Node Package Manager) installed.

- Create a New React App: by running:
   ```
   npx create-react-app jsx-lab
   cd jsx-lab
   ```

### Step 2: Create a Simple Component**

1. **Create a New Component:**
   Open the `src` folder in your project directory. Inside the `src` folder, create a new file named `SimpleComponent.js`.

2. **Write the Component:**
   Open `SimpleComponent.js` and write the following code:

   ```jsx
   import React from 'react';

   // Defining a simple functional component
   function SimpleComponent() {
       return (
           <div>
               <h1>Hello, JSX Lab!</h1>
               <p>This is a simple React component using JSX.</p>
           </div>
       );
   }

   // Export the component
   export default SimpleComponent;
   ```

### Step 3: Display the Component

1. **Open `src/index.js`:**
   Open the `src/index.js` file and replace the existing code with the following:

   ```jsx
   import React from 'react';
   import ReactDOM from 'react-dom';
   import SimpleComponent from './SimpleComponent';

   ReactDOM.render(
       <React.StrictMode>
           <SimpleComponent />
       </React.StrictMode>,
       document.getElementById('root')
   );
   ```

**Step 4: Run the App**

1. **Start the App:**
   Save all your changes and return to the terminal. Make sure you're still in the `jsx-lab` directory. Start the app by running:
   ```
   npm start
   ```

2. **View in Browser:**
   Your app will automatically open in your default web browser. You should see the output of your `SimpleComponent`.

**Summary:**

In this lab, you learned how to create a basic React component using JSX. You explored importing and exporting components, compared JSX to HTML, and gained a better understanding of how React mixes markup with rendering logic. You also learned how to display information with JSX and the importance of not passing JavaScript directly in JSX using curly braces.