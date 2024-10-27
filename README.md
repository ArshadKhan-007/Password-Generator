# Password Generator 🔐
A simple and customizable password generator built with React. This tool allows users to generate random passwords of a desired length, with optional inclusion of numbers and special characters.

## Features
Generate a random password with adjustable length (from 8 to 32 characters).
Toggle options to include numbers and/or special characters.
Copy generated password to clipboard with a single click.
Demo


##Technologies Used
React: For the user interface and state management.
Hooks: Utilizes useState, useEffect, useCallback, and useRef for state management, memoized functions, side effects, and direct DOM manipulation.
### Installation
Clone the repository:

bash
Copy code
git clone https://github.com/yourusername/password-generator.git
cd password-generator
Install dependencies:

bash
Copy code
npm install
Run the app:

bash
Copy code
npm start
The app should now be running on http://localhost:3000.

### Usage
Set Password Length: Use the range slider to select a length between 8 and 32 characters.

Include Numbers: Check the "Numbers" option to include digits (0-9) in the password.

Include Special Characters: Check the "Characters" option to include special symbols like !@#$%^&*()_+~.

Generate Password: The password updates automatically when any option changes.

Copy Password: Click the "COPY" button to copy the generated password to your clipboard.
## Code Overview
Components and Hooks
useState: Manages the state for length, numberAllowed, characterAllowed, and password.

useRef: Creates a reference to the password input for easy copying.


useCallback: Wraps passwordGenerator and copyPasswordToClipboard functions to memoize and optimize performance.

useEffect: Regenerates the password automatically when any dependency (length, numberAllowed, characterAllowed) changes.
### Main Functions
passwordGenerator: Generates a random password based on selected options.
copyPasswordToClipboard: Copies the generated password directly to the user's clipboard.
### Contributing
Feel free to open issues or submit pull requests if you find any bugs or have suggestions for new features.

### Fork the project.
Create your feature branch (git checkout -b feature/NewFeature).
Commit your changes (git commit -m 'Add new feature').
Push to the branch (git push origin feature/NewFeature).
Open a pull request.
License
Distributed under the MIT License. See LICENSE for more information.

