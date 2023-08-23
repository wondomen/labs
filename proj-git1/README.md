# Lab: Getting Started with Git: `init`, `commit`, and Basic Operations

In this lab, you'll get hands-on experience with the fundamental Git commands: `init` to initialize a new Git repository, and `commit` to save changes to your repository's history. You'll also learn about basic Git operations and workflows.

**Step 1: Setting Up Your Environment**

1. **Create a New Project Directory:**
   Open your terminal and navigate to a directory where you want to create your project. Create a new folder for your project using:
   ```
   mkdir git-basics-lab
   cd git-basics-lab
   ```

**Step 2: Initializing a Git Repository**

1. **Initialize Git Repository:**
   Run the following command to initialize a new Git repository in your project folder:
   ```
   git init
   ```

**Step 3: Making and Committing Changes**

1. **Create Files:**
   Create a new file named `README.md` in your project folder. Open the file in a text editor and add some content, e.g. "Welcome to My Git Basics Lab."

2. **Stage Changes:**
   Use the following command to stage the changes you've made:
   ```
   git add README.md
   ```

3. **Commit Changes:**
   Commit the staged changes with a descriptive message using the following command:
   ```
   git commit -m "Initial commit: Added README.md"
   ```

**Step 4: Basic Git Operations**

1. **View Repository Status:**
   Use the following command to see the current status of your repository:
   ```
   git status
   ```

2. **View Commit History:**
   View the commit history to see your commit using:
   ```
   git log
   ```

**Step 5: Making and Committing More Changes**

1. **Modify `README.md`:**
   Open `README.md` again in a text editor and make some changes to the content.

2. **Stage and Commit Changes:**
   Repeat the steps to stage and commit the changes you've made to `README.md`.

**Step 6: Create a New File and Commit**

1. **Create a New File:**
   Create a new file named `index.html` in your project folder. Add some simple HTML content to the file.

2. **Stage and Commit:**
   Stage and commit the new file `index.html` with an appropriate message.

**Summary:**

In this lab, you got hands-on experience with Git's core commands: `init` to initialize a Git repository, and `add` and `commit` to track and save changes. You also learned how to view the status of your repository and the commit history. This foundational knowledge will serve as the basis for more advanced Git workflows and collaborative development.