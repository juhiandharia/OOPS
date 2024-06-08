# Bank Account Management System

This project is a simple Bank Account Management System implemented in C++. It allows users to open a new account, add cash to an existing account, and withdraw cash from an existing account. The account details are stored in a text file for persistence.

## Features

1. **Open New Account**: Allows a user to create a new bank account with an account number and a strong password. The initial balance is set to zero.
2. **Add Cash**: Enables a user to add cash to their existing bank account by providing the account number.
3. **Withdraw Cash**: Allows a user to withdraw cash from their existing bank account by providing the account number and password.

## Files

- **Account.txt**: This file stores the account details including account number, password, and balance.
- **Account Temp.txt**: A temporary file used for updating account details.

## Classes

### Account

- **Private Members**:
  - `string AccountNo`
  - `string Password`
  - `int Balance`

- **Public Methods**:
  - `void setAccountNo(string id)`
  - `void setPassword(string pw)`
  - `void setBalance(int balance)`
  - `string getAccountNo()`
  - `string getPassword()`
  - `int getBalance()`

## Functions

### openAccount(Account user)

Prompts the user to enter an account number and a strong password to create a new account. Initializes the balance to zero and saves the account details in `Account.txt`.

### addCash()

Prompts the user to enter their account number and the amount of cash to add. Updates the balance in `Account.txt`.

### withdraw()

Prompts the user to enter their account number and password, then the amount of cash to withdraw. Checks if the balance is sufficient and updates the balance in `Account.txt`.

## Main Function

The main function provides a simple text-based interface for the user to interact with the system. It allows the user to choose one of the following options:

1. Open a new account
2. Add cash to an account
3. Withdraw cash from an account
4. Exit the system

## How to Run

1. Compile the C++ code using a compiler like `g++`.

   ```sh
   g++ -o BankAccountManagement main.cpp
