# Coding Exercise Environment Setup Guide (macOS)

Follow these steps to set up your environment for the coding exercise.

## 1. Install Python

1. Open Terminal (`Cmd + Space`, type "Terminal", press Enter).
2. Install Homebrew (if not already installed):
   ```zsh
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```
3. Install Python:
   ```zsh
   brew install python
   ```
4. Verify installation:
   ```zsh
   python3 --version
   ```

## 2. Install Visual Studio Code

1. Go to [VS Code Download Page](https://code.visualstudio.com/Download).
2. Download the macOS version and install it by dragging the app to your Applications folder.
3. Open VS Code from Applications.

## 3. Set Up a Python Virtual Environment

1. In Terminal, navigate to your project directory (or create one):
   ```zsh
   mkdir ~/coding-exercise
   cd ~/coding-exercise
   ```
2. Create a virtual environment:
   ```zsh
   python3 -m venv venv
   ```
3. Activate the virtual environment:
   ```zsh
   source venv/bin/activate
   ```
4. Upgrade pip:
   ```zsh
   pip install --upgrade pip
   ```
5. Install required packages:
   ```zsh
   pip install matplotlib pandas seaborn tabulate
   ```

## 4. Clone the GitHub Repository

1. Install Git (if not already installed):
   ```zsh
   brew install git
   ```
2. Clone the repository (replace `<URL>` with the actual repo URL):
   ```zsh
   git clone <URL>
   cd <repo-folder>
   ```

## 5. Open the Project in VS Code

1. In Terminal, inside the project folder, run:
   ```zsh
   code .
   ```
   (If `code` command is not found, open VS Code, press `Cmd+Shift+P`, type "Shell Command: Install 'code' command in PATH", and select it.)

---
