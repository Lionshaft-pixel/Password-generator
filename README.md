# Password Generator

[![Technology](https://img.shields.io/badge/Language-JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

A simple yet robust random password generator built with JavaScript. This tool allows users to create strong, secure passwords by combining various character types including symbols, numbers, uppercase letters, and lowercase letters, enhancing online security.

---

## Key Features & Benefits

*   **Highly Customizable:** Generate passwords with precise control over character sets:
    *   Lowercase characters (a-z)
    *   Uppercase characters (A-Z)
    *   Numbers (0-9)
    *   Symbols (!@#$%^&*()_+=-\)
*   **Strong Security:** Produces genuinely random passwords, making them difficult to guess or crack.
*   **Lightweight & Client-Side:** Implemented purely in JavaScript, running directly in the browser without server interaction.
*   **Educational Tool:** A great example of basic JavaScript functionality for string manipulation and random number generation.

---

## Prerequisites & Dependencies

To run this project, you only need:

*   A modern web browser (e.g., Chrome, Firefox, Edge, Safari) capable of executing JavaScript.

This project has no external library dependencies.

---

## Installation & Setup

Follow these simple steps to get the password generator running on your local machine:

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Lionshaft-pixel/Password-generator.git
    cd Password-generator
    ```

2.  **Open in your browser:**
    Simply open the `index.html` file in your preferred web browser. You can do this by navigating to the file in your file explorer and double-clicking it, or by using a command like:
    ```bash
    open index.html # On macOS
    start index.html # On Windows
    xdg-open index.html # On Linux
    ```
    *Note: The current implementation provides a JavaScript function (`generatePassword`) that can be called from the browser's developer console. Future updates might include a graphical user interface (GUI) for easier interaction.*

---

## Usage

The core functionality is provided by the `generatePassword` JavaScript function. You can call this function from your browser's developer console to generate passwords.

### `generatePassword(length, includeLowerCase, includeUpperCase, includeNumbers, includeSymbols)`

**Parameters:**

*   `length` (Number, required): The desired length of the password.
*   `includeLowerCase` (Boolean, optional): Set `true` to include lowercase letters (a-z)
*   `includeUpperCase` (Boolean, optional): Set `true` to include uppercase letters (A-Z)
*   `includeNumbers` (Boolean, optional): Set `true` to include numbers (0-9)
*   `includeSymbols` (Boolean, optional): Set `true` to include symbols (!@#$%^&*()_+=-\)

**Returns:**

*   A `String` representing the generated password.

**Example (using browser console):**

To open the developer console in most browsers:
*   Windows/Linux: `F12` or `Ctrl+Shift+I`
*   macOS: `Cmd+Option+I`

Once the console is open, you can call the function:

```javascript
// Generate a 12-character password with lowercase, uppercase, numbers, and symbols
generatePassword(12, true, true, true, true);
// Expected output: "example!P9xZ$" (will vary)

// Generate a 10-character password with only lowercase and numbers
generatePassword(10, true, false, true, false);
// Expected output: "h5g2j8k1m0" (will vary)

// Attempt to generate a password with no character types selected
generatePassword(8, false, false, false, false);
// Expected output: An error or an empty string, as no characters are allowed
```

---

## 🛠️ Configuration Options

The `generatePassword` function itself serves as the primary configuration mechanism. By adjusting its parameters, you can customize the password generation process to meet specific requirements:

| Parameter          | Type      | Description                                                    | Default (Implied) |
| :----------------- | :-------- | :------------------------------------------------------------- | :---------------- |
| `length`           | `Number`  | The total number of characters in the generated password.      | (User Defined)    |
| `includeLowerCase` | `Boolean` | Include `a-z` in the password.                                 | `false`           |
| `includeUpperCase` | `Boolean` | Include `A-Z` in the password.                                 | `false`           |
| `includeNumbers`   | `Boolean` | Include `0-9` in the password.                                 | `false`           |
| `includeSymbols`   | `Boolean` | Include `!@#$%^&*()_+=-\` in the password.                    | `false`           |

---

## 🤝 Contributing

This repo doesn't really have much to add but if you really have some suggestions for new features, bug fixes, or improvements, I won't mind. Just follow these steps:

1.  **Fork** the repository.
2.  **Create a new branch** for your feature or bug fix:
    ```bash
    git checkout -b feature/your-feature-name
    # or
    git checkout -b bugfix/issue-description
    ```
3.  **Make your changes** and ensure the code adheres to existing style.
4.  **Commit your changes** with a clear and descriptive message.
5.  **Push your branch** to your forked repository.
6.  **Open a Pull Request** to the `main` branch of this repository, describing your changes and their benefits.

### Ideas for Contribution:
*   Implement a simple HTML/CSS user interface (UI) to interact with the `generatePassword` function.
*   Add options for custom symbol sets.
*   Improve error handling (e.g., if no character types are selected).
*   Refactor the code for better modularity or performance.

---

## License

You can have it, I don't really care. The best you can do is just give me credits. That's all.

---

## 🙏 Acknowledgments

This project was developed by [Lionshaft-pixel](https://github.com/Lionshaft-pixel) as part of a learning journey in JavaScript. Special thanks for the foundational knowledge gained during the learning process.
