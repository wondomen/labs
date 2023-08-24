# Lab: Working with Props in React

In this lab, you'll create a React component and explore how to pass, read, and manage props.

**Step 1: Setting Up Your Environment**

1. **Create a New React App:**

- Create a New React App based on this simple template 

```sh
npx degit tx00-web/labs/react-starter#main props-lab
cd props-lab
```

> [degit] clones a specific subdirectory instead of the entire repo.

**Step 2: Create and Use a Component with Props**

1. **Create a New Component:**
   Open the `src` folder in your project directory. Inside the `src` folder, create a new file named `WelcomeMessage.js`.

2. **Write the Component:**
   Open `WelcomeMessage.js` and write the following code:

   ```jsx
   // Defining a functional component with props
   function WelcomeMessage(props) {
       return (
           <div>
               <h1>Welcome, {props.name}!</h1>
               <p>{props.message}</p>
               {props.children}
           </div>
       );
   }

   export default WelcomeMessage;
   ```

**Step 3: Using the Component and Passing Props**

1. **Open `src/App.js`:**
   Open the `src/App.js` file and replace the existing code with the following:

   ```jsx
   import WelcomeMessage from './WelcomeMessage';

   function App() {
       return (
           <div className="App">
               <WelcomeMessage name="Alice" message="This is a welcome message">
                   <p>This is some additional JSX passed as children.</p>
               </WelcomeMessage>
           </div>
       );
   }

   export default App;
   ```

**Step 4: Run the App**

1. **Start the App:**
   Save all your changes and return to the terminal. Make sure you're still in the `props-lab` directory. Start the app by running:
   ```
   npm start
   ```

2. **View in Browser:**
   Your app will automatically open in your default web browser. You should see the output of the `WelcomeMessage` component, which displays the name, message, and additional JSX passed as children.

**Summary:**

In this lab, you learned how to work with props in React components. You created a component that accepts props, passed props to the component, and learned how to read and use those props. You also saw how to provide default values for props and how to pass additional JSX as children. Finally, you explored how props can change over time, making your components dynamic and flexible.

<!-- Links -->
[degit]:https://github.com/Rich-Harris/degit