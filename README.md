# DBank Project

## Overview

DBank is a simple web-based banking application that allows users to manage their account balance by depositing and withdrawing funds. The application uses the Internet Computer's Motoko programming language for backend logic, and basic HTML, CSS, and JavaScript for the frontend. It features real-time balance updates and a compound interest function that calculates interest based on the time elapsed since the last interaction.

## Features

- **Top Up**: Add funds to your balance.
- **Withdraw**: Remove funds from your balance.
- **Compound Interest**: Automatically apply compound interest to the balance over time.
- **Real-Time Balance Update**: View your updated balance instantly after any transaction.

## Motoko Backend (`main.mo`)

This file contains an actor `DBank` with:
- A stable variable for storing the current balance.
- Methods for depositing (`topUp`), withdrawing (`withdraw`), and checking the balance (`checkBalance`).
- A compound interest method (`compound`) that updates the balance based on the time elapsed.

## Frontend (`index.html`, `index.js`)

The HTML file sets up the user interface. JavaScript handles the interaction between the frontend and the Motoko backend, updating the UI based on user actions and backend responses.

![image](https://github.com/Nazym-MU/dbank/assets/150896747/c24e3b2f-aa14-4ac9-9b91-fa6c1d692037)

## Setup and Running

1. **Clone the repository:**

```
git clone <repository-url>
```
2. **Navigate to the project directory:**
```
cd dbank
```
3. **Install dependencies:**
```
npm i
```
4. **Run the project locally:**
```
dfx start --background
dfx deploy
npm start
```
5. **Open your web browser and go to:**
http://localhost:8080

## Dependencies

- Node.js and npm
- DFINITY Canister SDK (dfx)

## Contributing

Contributions to DBank are welcome! Please refer to the contributing guidelines before making pull requests.