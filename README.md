# Password Generator & Validator

A simple command-line Python program that can either generate a random password based on your preferences or check whether a password you type meets basic strength rules.

## Features

- Generate a random password of a custom length (minimum 4 characters)
- Choose whether to include uppercase letters, numbers, and special characters
- Validate your own password against these rules:
  - At least 8 characters long
  - At least one letter
  - At least one special character
- Clear feedback listing exactly which rules a password fails
- Input validation with friendly error messages
- Type `exit` at the main menu to quit

## Requirements

- Python 3.6 or higher
- No external libraries needed (uses only the built-in `random` and `string` modules)

## How to Run

1. Clone the repository:
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>

2. Run the program:
   python password_generator.py

(Replace `password_generator.py` with your actual file name.)

## Usage

1. Start the program and type `yes` to continue.
2. Choose whether to enter your own password:
   - yes: type a password and the program checks it against the rules.
   - no: the program asks for length and character options, then generates a password.
3. Type `exit` when you want to quit.

## Example

Welcome to the Password Generator!
Do you want to continue? (yes to proceed, exit to quit): yes
Do you want to enter your own password? (yes/no): no
Enter the desired password length: 12
Include uppercase letters? (yes/no): yes
Include numbers? (yes/no): yes
Include special characters? (yes/no): yes
Your generated password is: k#9Tq!vB2@zL

## How It Works

- generate_password(): builds a character pool from your choices and picks random characters from it.
- validate_password(): checks length, letters, and special characters, and returns a list of any unmet criteria.
- The main loop handles the menu and user input.

## Security Note

This project uses Python's `random` module, which is fine for learning and practice but is not cryptographically secure. For real-world passwords, consider using the `secrets` module instead.

## License

This project is open source and free to use for learning purposes.
