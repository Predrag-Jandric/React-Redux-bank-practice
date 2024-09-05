# React (Redux) - bank app

# 🔗 [Live Preview]()

![Design preview]()

---

## About Project 👋

This small practice app's main goal is to practice using managing global state using redux toolkit and vanilla redux. It allows users to deposit or withdraw money, request and repay loans into their bank accounts. It also supports simple customer creation, so new users can quickly set up their accounts.


Created using create-react-app

---

## Features 👨‍💻

-   **Create New Customer:** Enter your full name and national ID to create a new customer profile. This is the first step before accessing any account operations.

    -   **Account Operations:**

    -   **Deposit Money:** Add money to your account in different currencies, and it will be automatically converted to USD.

    -   **Withdraw Money:** Take money out of your account at any time.

    -   **Request a Loan:** Apply for a loan by specifying the amount and purpose. If approved, the loan amount will be added to your balance.

    -   **Pay Back Loan:** Repay your loan once you have the funds available.
    
    -   **Balance Display:** Always stay informed about your account balance, displayed in USD for easy understanding.

---

## How it works ⚙️


1.  **App Component:**
    -   This is the main component that renders either the customer creation form or the account operations and balance display based on whether a customer has been created.

2.  **CreateCustomer Component:**
    -   Handles the creation of a new customer by taking inputs for full name and national ID. Dispatches the `createCustomer` action to store the customer's information in the Redux store.

3.  **Customer Component:**
    -   Displays a welcome message with the customer's name once they have been created.

4.  **AccountOperations Component:**
    -   This component provides a user interface for performing account operations like deposits, withdrawals, loan requests, and loan payments. It interacts with the Redux store to dispatch relevant actions.

5.  **BalanceDisplay Component:**
    -   Displays the user's current balance in USD. This component pulls data from the Redux store to ensure accurate and real-time information.

### State Management

-   **Redux Store:**

    -   The app uses Redux for state management, with two main slices: `accountSlice` and `customerSlice`.

-   **Account Slice:**
    -   Manages the balance, loan details, and loading states related to currency conversion.
    -   Actions include `deposit`, `withdraw`, `requestLoan`, and `payLoan`.

-   **Customer Slice:**
    -   Handles customer details like full name, national ID, and creation date.
    -   Actions include `createCustomer` and `updateName`.

This structure allows for efficient and centralized management of the app's state, making it easy to track and update account and customer information as needed.

---

## Technologies & Dependencies used 📦

- **React:** components, conditionals, functions... 

- **Redux:** store, slices, reducers 

- **Styling:** basic CSS 

dependencies:

- /dependence:/ /version number/
- /dependence:/ /version number/
- /dependence:/ /version number/

devDependencies:

- /dependence:/ /version number/
- /dependence:/ /version number/
- /dependence:/ /version number/

---

## Prerequisites 📚

Ensure you have the following installed on your system:

    Node.js v18.00.0
    npm or yarn

---

## Clone & Run locally 🏃‍♂️

1. **Clone the Repository:**

   - On the GitHub repo page, click the green "Code" button.

   - Copy the HTTPS URL.

2. **Open the Terminal:**

   - Open the terminal by typing "cmd" in your desktop's start menu, **OR**

   - Right-click on the desktop and select "Git Bash Here" (if you have Git Bash installed), **OR**

   - Open Visual Studio Code's terminal by clicking "Terminal" -> "New Terminal" inside the editor.

3. **Navigate to Your Project Location:**

   - In the terminal, navigate to your desired location (e.g., desktop) using the command: `cd desktop`. Adjust the path if your project is located elsewhere.

   - Ensure that your terminal's address is inside the project folder.

4. **Clone the Repository:**

   - Run the command: `git clone /link/`. Replace `/link/` with the HTTPS URL from step 1.

5. **Enter the Project Directory:**

   - Navigate into the cloned repository by typing: `cd /folder-name/`. Replace `/folder-name/` with the name of the cloned folder.

6. **Install Dependencies:**

   - Run the command: `npm install` to install all the necessary dependencies.

7. **Start the Project:**

   - Run the command: `npm start` or `yarn start` to start the project. It will open in your default browser at [localhost:3000/](http://localhost:3000/)

---

## Project Structure 📂

    project-name
    ├── public 
    ├── src
    │ ├── features 
    │ │ ├── account 
    │ │ │   ├── AccountOperations.js 
    │ │ │   ├── accountSlice.js 
    │ │ │   ├── BalanceDisplay.js  
    │ │ ├── customers 
    │ │ │   ├── createCustomer.js 
    │ │ │   ├── customer.js  
    │ │ │   ├── customerSlice.js     
    │ ├── App.js 
    │ ├── index.css 
    │ ├── index.js 
    │ ├── store-v1 
    │ ├── store-v2 
    │ ├── store.js 
    ├── package.json 
    └── README.md 

---

## Contributing 💻

Contributions are closed.