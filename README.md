# ATM Application

This is a simple command-line ATM application implemented in Python. It allows users to register, login, check their balance, deposit funds, and withdraw funds. The application simulates basic banking operations in an interactive and user-friendly manner.

## Features

- **User Registration**: New users can register by providing a username, password, and an initial deposit.
- **User Authentication**: Users can login with their username and password.
- **Check Balance**: Users can check their current account balance.
- **Deposit Funds**: Users can deposit funds into their account.
- **Withdraw Funds**: Users can withdraw funds from their account, subject to having sufficient balance.
- **Logout**: Users can logout of their session.

## Classes and Methods

### `User` Class
Represents a bank user with the following methods:
- `__init__(username, password, balance)`: Initializes a new user with a username, password, and balance.
- `check_balance()`: Prints the user's current balance.
- `deposit(amount)`: Deposits a specified amount into the user's account.
- `withdraw(amount)`: Withdraws a specified amount from the user's account if sufficient balance is available.

### `ATM` Class
Manages user operations with the following methods:
- `__init__()`: Initializes the ATM with a predefined set of users.
- `add_user(username, password, balance)`: Adds a new user to the ATM.
- `validate(username, password)`: Validates user credentials and returns the user object if successful.
- `register_user()`: Prompts for new user registration details and adds the user.

### Main Application Loop
The `main()` function handles the main menu and user interactions:
- **Register**: Allows new users to register.
- **Login**: Allows existing users to login and perform banking operations.
- **Exit**: Exits the application.
