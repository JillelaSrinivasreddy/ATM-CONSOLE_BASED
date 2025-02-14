# ATM-CONSOLE_BASED

This is a simple ATM system implemented in Python, offering features like balance checking, withdrawals, deposits, pin generation, and mini statements. The application works with user data stored in a dictionary, where each account is represented by a unique account number.

## Features

- **Withdrawal**: Allows users to withdraw money if the correct pin is entered and if there's sufficient balance.
- **Deposit**: Users can deposit funds into their account.
- **Pin Generation/Change**: Users can generate a new pin or change their existing pin.
- **Mini Statement**: View account details including balance, name, and email.
- **Exit**: Exit the program safely.

## Requirements

- Python 3.x or higher
- Text-based terminal (Command Prompt, Terminal, etc.)

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/ATM-console-based.git
    ```

2. Navigate to the project directory:
    ```bash
    cd ATM-console-based
    ```

3. No external dependencies are required for this project, as it uses standard Python libraries.

4. Run the application:
    ```bash
    python atm.py
    ```

## Usage

1. On running the script, the user will be prompted to choose from the following options:
    - Withdrawal
    - Deposit
    - Pin Generation
    - Mini Statement
    - Exit

2. **Withdrawal**: Enter the account number and pin. Then specify the amount to withdraw. The transaction will only proceed if there's enough balance in the account.
   
3. **Deposit**: Enter the account number and the amount to deposit. The balance will be updated accordingly.
   
4. **Pin Generation/Change**: If a pin is already generated, the user can change it. If no pin is generated, a new pin will be set.

5. **Mini Statement**: Enter your account number and pin to view your account details such as balance, name, and email.

6. **Exit**: Close the application.

## Code Structure

- `atm.py`: The main Python script that contains the core logic of the ATM system. It uses a dictionary `accounts` to store user details:
    - Account number
    - Balance
    - Pin (if generated)
    - Email
    - Name

### Example Data
```python
accounts = {
    5573: [2000, 2580, "jsrinivasreddy350@gmail.com", "J Srinivasreddy"],
    6308: [4000, 5573, "manikantareddy123@gmail.com", "CH Manikanta"],
    9347: [3000, 9890, "jkrishnareddy567@gmail.com", "J Krishna reddy"],
    9502: [5000, None, "jvenkatreddy890@gmail.com", "J Venkatreddy"]
}
