# ATM Machine Project

## Overview:
This project demonstrates the development of an ATM (Automated Teller Machine) system, implemented using C# and SQL for database management. The project aims to simulate the functionalities of a real ATM, such as account authentication, balance checks, deposit and withdrawal operations, transaction history, and user account management.

## Features:
- **User Authentication**: Customers can log in using a PIN and account number.
- **Balance Inquiry**: Users can check their current account balance.
- **Withdraw and Deposit**: Allows for cash withdrawals and deposits with proper validation and balance update.
- **Transaction History**: View a list of recent transactions.
- **Database Management**: All user information, transactions, and balances are securely stored in an SQL database.

## Technologies Used:
- **C#**: The core programming language for implementing the ATM functionality.
- **SQL**: Database management system used for storing user data, transactions, and account balances.
- **Visual Studio**: Integrated Development Environment (IDE) used to build and test the application.
- **DBMS Concepts**: To manage database connections, queries, and transaction handling.

## Installation Instructions:
1. **Prerequisites**:
   - Install **Visual Studio** (Community Edition is sufficient).
   - Set up **SQL Server** (LocalDB or full SQL Server instance) to run the database.
   
2. **Clone or Download the Repository**:
   - Clone this repository to your local machine or download the files as a ZIP.

3. **Setting Up the Database**:
   - Open **SQL Server Management Studio (SSMS)** or **SQL Server Object Explorer** in Visual Studio.
   - Run the SQL scripts located in the `Database/` folder to create the necessary tables and stored procedures for the ATM system.
   - Ensure the connection string in the C# project points to the correct SQL server instance.

4. **Running the Project**:
   - Open the project in **Visual Studio**.
   - Build the project by pressing **Ctrl+Shift+B**.
   - Run the application by pressing **F5** or **Ctrl+F5**.
   - Follow the on-screen instructions to interact with the ATM system.

## Usage Instructions:
- When the ATM system starts, the user will be prompted to enter their **Account Number** and **PIN**.
- After successful login, the user will have the option to:
  - Check the balance
  - Withdraw funds (ensuring sufficient balance)
  - Deposit funds
  - View transaction history
- All actions will be reflected in the **SQL database**, and users can query the database for records of their transactions.

## Code Structure:
- **ATM.cs**: Contains the main logic for the ATM operations (authentication, deposit, withdrawal, etc.).
- **DatabaseHelper.cs**: Handles database connection and SQL queries.
- **SQL Scripts**: Includes the schema for creating tables like `Users`, `Transactions`, and `Accounts`.
- **UI**: Console-based interface for user interaction (can be upgraded to a GUI if desired).

## Future Improvements:
- Improve already Implemented **GUI** using Windows Forms or WPF for a more user-friendly experience.
- Add **encryption** for PINs and account data for enhanced security.
- Implement **multi-account support** for a more complex simulation of ATM behavior.

## License:
This project is open-source. Feel free to modify, use, and distribute as needed.
