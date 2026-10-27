# Mini-Git 🧩
### A Lightweight Version Control System Built with Python

Mini-Git is a command-line project that explores the fundamentals of version control by implementing basic repository operations using Python and filesystem storage.

## 📌 Project Overview

Version control systems help developers manage changes, maintain project history, and organize parallel development. Mini-Git explores these concepts through a simplified implementation of commits, branches, references, and history navigation.

The project focuses on understanding how repository data can be organized and managed without relying on Git internally.

## ✨ Features

- **Repository Initialization** — Set up the directory structure for storing version control data.
- **Commit Creation** — Record commits with descriptive messages.
- **Branch Management** — Create branches to maintain separate development paths.
- **Branch Switching** — Change the currently active branch.
- **Commit References** — Track commit pointers and branch history.
- **History Navigation** — Navigate to an earlier commit within a branch.
- **Filesystem Storage** — Organize commit-related data in local directories.

## 🗂️ Directory Structure

```text
mini-git/
├── obj/                 # Commit object storage
├── ref/
│   └── branches/        # Branch references and history
├── crntBranch           # Active branch tracker
├── init.py              # Repository setup
├── commit.py            # Commit command
├── createcommit.py      # Commit creation logic
├── createBranch.py      # Branch creation
├── getBack.py           # Previous commit navigation
└── switch-branch.py     # Branch switching
```

## ⚙️ Installation and Usage

### Prerequisites

- Python 3.x
- A terminal or command prompt

### Initialize the Repository

```bash
python init.py
```

### Create a Commit

```bash
python commit.py -m "Initial commit"
```

### Create a New Branch

```bash
python createBranch.py "feature"
```

### Switch to Another Branch

```bash
python switch-branch.py "feature"
```

### Navigate to an Earlier Commit

```bash
python getBack.py "commit message"
```

Run these commands from the project directory. The available operations and their exact behavior depend on the implementation of each script.

## 🧠 Design Principles

Mini-Git organizes repository information using directories, files, and references.

- **Commit Tracking:** Commit-related information is maintained locally.
- **Branch References:** Each branch has references that identify its commit state.
- **Active Branch Management:** A dedicated file tracks the current branch.
- **History Management:** Branch-specific files maintain commit history.
- **Modular Structure:** Different Python scripts handle individual repository operations.

Together, these components demonstrate how basic version control functionality can be represented through filesystem operations.

## 🎯 Learning Objectives

This project explores:

- Version control fundamentals
- Commit and branch relationships
- Filesystem-based data organization
- Reference and pointer management
- Python scripting and command-line interfaces
- Modular program design

