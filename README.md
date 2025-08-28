# Java DevContainer Template

A **ready-to-use Java project template** for Visual Studio Code with [Dev Containers](https://code.visualstudio.com/docs/devcontainers/containers).
This template aims to provide a clean project structure, consistent build environment, and easy-to-run VS Code tasks.

---

## 📌 Project Goal

The goal of this repository is to provide a **clone-and-code Java workflow** that works out of the box.
It eliminates the hassle of setting up IDE extensions, environment variables, or custom scripts by including:

* 🐳 **DevContainer support** (Docker-based reproducible environment)
* ⚡ **VS Code tasks** for compiling and running Java without retyping long `javac` commands
* 📂 **Project structure** (`src/`, `lib/`, `bin/`) that mirrors common Java practices
* 📦 **Dependency support** via `lib/` for JARs

---

## 🚀 Getting Started

### 1. Clone the Template

```bash
git clone https://github.com/Richard-Hathaway/java-devcontainer-template.git
cd java-devcontainer-template
```

### 2. Open in VS Code

Open the project in VS Code. When prompted, reopen in the Dev Container.

### 3. Compile & Run

Place `.java` files inside the `src/` directory.
Place `.jar` dependencies inside the `lib/` directory.

Use the **default VS Code build task** (⇧⌘B / Ctrl+Shift+B) to compile.
Compiled `.class` files will be placed in `bin/`.

Run your program with:

```bash
java -cp "bin:lib/*" MainClassName
```

---

## 🗂 Project Structure

```
.devcontainer/   # Dev Container setup (Dockerfile, config)
.vscode/         # VS Code settings and tasks
bin/             # Compiled .class files (ignored in Git)
lib/             # External .jar dependencies
src/             # Your Java source files
```

---

## ⚙️ Requirements

* [Docker](https://www.docker.com/get-started) installed and running
* [Visual Studio Code](https://code.visualstudio.com/) with the **Dev Containers** extension

---

## 📜 License

MIT License — feel free to use, modify, and distribute.

---

## 🙌 Contributions

Pull requests and suggestions are welcome!
Open an issue if you have ideas for improvements.
