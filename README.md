<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Visual_Studio_Code_1.35_icon.svg" width="100" alt="IDE Tutor Logo" />
</p>

<h1 align="center">IDE Tutor: Professional Cloud Development Workspace</h1>

<p align="center">
  <b>A high-fidelity, zero-dependency VS Code clone for Google Apps Script.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Version-2.0.0-blue.svg" alt="Version" />
  <img src="https://img.shields.io/badge/Platform-Google%20Apps%20Script-green.svg" alt="Platform" />
  <img src="https://img.shields.io/badge/License-MIT-orange.svg" alt="License" />
  <img src="https://img.shields.io/badge/Vanilla-JS-yellow.svg" alt="Vanilla JS" />
</p>

---

## 🌟 Overview

**IDE Tutor** is a sophisticated, browser-based integrated development environment (IDE) built entirely with Vanilla JavaScript, CSS3, and HTML5. It provides a near-native VS Code experience within the Google Apps Script ecosystem, featuring a persistent virtual file system, multi-language transpilation, and a modern, customizable UI.

Designed for educators, students, and developers, it offers a "zero-setup" environment for practicing multiple programming languages directly in the cloud without external dependencies or CDNs.

## 🚀 Key Features

### 💻 High-Fidelity VS Code Interface
*   **Modern Aesthetic**: Fully responsive layout with custom themes (Dark+, Monokai, Dracula, Solarized).
*   **Standard Layout**: Activity Bar, Sidebar, Editor Pane, Command Palette, and Status Bar.
*   **IntelliSense & Snippets**: Context-aware suggestions and code snippets for over 10 languages.
*   **Advanced Editor**: Custom-built text editor with sync-scrolling line numbers, tab-interception, and smart indentation.

### 📂 Persistent Virtual File System (VFS)
*   **Cloud Storage**: Native persistence using Google's `PropertiesService`.
*   **File Management**: Create, delete, and rename files dynamically.
*   **State Persistence**: Open tabs and active files are remembered across sessions.

### ⚙️ Multi-Language Execution Engine
The IDE features a custom-built transpilation layer that maps various languages to JavaScript for browser-side execution:
*   **JavaScript (ES6+)**: Direct execution with instrumentation.
*   **Python**: Transpiles loops, conditionals, and standard I/O (using `prompt` for input).
*   **C++**: Simulates `iostream` (`cout`, `cin`) and standard variable declarations.
*   **Java**: Advanced simulation including **concurrency mocks** (`AtomicInteger`, `ExecutorService`, `TimeUnit`) and lambda expressions.
*   **Web Technologies**: Live preview for HTML and CSS files in a dedicated iframe.
*   **Additional Support**: Syntax highlighting and snippets for Rust, Go, Ruby, and SQL.

## 🛠 Tech Stack

*   **Backend**: Google Apps Script (V8 Engine).
*   **Frontend**: Vanilla HTML5, CSS3 (using CSS Variables for themes), and ES6+ JavaScript.
*   **Tooling**: Managed via `@google/clasp` for streamlined deployment and version control.

## 📦 Installation & Deployment

To deploy your own instance of IDE Tutor:

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/Cancelllls/IDE-Tutor.git
    cd IDE-Tutor
    ```

2.  **Authenticate Clasp**:
    ```bash
    npx clasp login
    ```

3.  **Create a New Script Project** (or link an existing one):
    ```bash
    npx clasp create --title "IDE Tutor" --type webapp
    ```

4.  **Push the Code**:
    ```bash
    npx clasp push
    ```

5.  **Deploy as Web App**:
    ```bash
    npx clasp deploy --description "Initial Release"
    ```

## 📖 Architecture Note

Unlike traditional IDEs that rely on heavy libraries like Monaco or Ace Editor, **IDE Tutor** is built from the ground up to be **zero-dependency**. The syntax highlighter, code editor, and language transpilers are all custom-implemented to ensure maximum performance and security within the Google Apps Script environment.

## 🤝 Contributing

Contributions are welcome! Whether it's adding a new language transpiler, improving the UI, or fixing bugs, feel free to fork the repo and submit a pull request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

<p align="center">
  Created with ❤️ by <a href="https://github.com/Cancelllls">Cancelllls</a>
</p>
