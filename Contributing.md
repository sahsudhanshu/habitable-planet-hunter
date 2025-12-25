# Contributing to Exoplanet Habitability Prediction

Thank you for your interest in contributing to this project! To ensure a smooth collaboration and maintain a high-quality codebase, please follow the guidelines below.

## 🛠 Getting Started

1.  **Fork the repository** to your own GitHub account.
2.  **Clone the project** to your local machine.
3.  **Set up the environment:**
    * Ensure you are using **Python 3.10** (as per the strict compatibility rules).
    * **Manage Dependencies:**
        * **Install:** Run `pip install -r requirements.txt` to install current dependencies.
        * **Create/Update:**
            * If `requirements.txt` does not exist, **create one**.
            * If you install **any** new libraries during development, you **must** update the file.
            * Run `pip freeze > requirements.txt` to capture the exact versions of all installed libraries before committing.

---

## 💻 Coding Standards

We strive for clean, readable, and reproducible code. Please adhere to the following rules:

### 1. Style & Formatting
* **PEP 8 Compliance:** Follow standard Python style guidelines. Use tools like `flake8` or `black` to format your code before committing.
* **Notebooks vs. Scripts:**
    * If submitting a **Jupyter Notebook**, ensure all cells are run in order and the output is visible.
    * Remove unused code cells or large commented-out blocks before submitting.
* **Variable Naming:** Use descriptive, snake_case variable names.
    * ✅ `planet_radius_earth_units`
    * ❌ `rad`, `p_r`, `x`

### 2. Documentation & Comments
* **Docstrings:** Every function and class must have a docstring explaining:
    * What it does.
    * The arguments (and their types).
    * The return value.
* **Inline Comments:** Use comments to explain *why* complex logic exists, not *what* the code is doing (the code should speak for itself).

### 3. Modularity
* Avoid hard-coding paths (e.g., `C:/Users/Name/Downloads/...`). Use relative paths.
* Break large functions into smaller, reusable components.

---

## 📝 Commit Message Guidelines

We follow the **Conventional Commits** specification to keep our history clean and readable.

### Format
`type: short description in imperative mood`

### Allowed Types
* `feat`: A new feature (e.g., adding a new visualization or model).
* `fix`: A bug fix (e.g., fixing data loading errors).
* `docs`: Documentation only changes.
* `style`: Changes that do not affect the meaning of the code (formatting, missing semi-colons, etc).
* `refactor`: A code change that neither fixes a bug nor adds a feature.
* `chore`: Maintenance tasks (e.g., updating requirements).

### Rules
1.  **Imperative Mood:** "Add feature" not "Added feature" or "Adding feature".
2.  **Length:** Keep the first line under 50 characters.
3.  **No Period:** Do not end the subject line with a period.

### Examples
* ✅ `feat: implement random forest classifier`
* ✅ `fix: handle missing values in stellar mass column`
* ✅ `docs: update readme with python 3.10 instructions`
* ✅ `chore: update requirements.txt with xgboost`
* ❌ `Added some code for the model` (Vague, wrong tense)

---

## 🚀 Pull Request (PR) Process

1.  **Create a Branch:** Always work on a new branch for your specific task.
    * `git checkout -b feat/feature-selection-logic`
2.  **Self-Review:** Review your own code before opening a PR. Remove temporary print statements and debug code.
3.  **Descriptive PR Title:** Your PR title should summarize the change clearly.
4.  **PR Description:** In the description, clearly state:
    * What changes were made.
    * Why they were made.
    * Any relevant issue numbers (e.g., `Closes #4`).

Thank you for contributing to better exoplanet prediction! 🪐
