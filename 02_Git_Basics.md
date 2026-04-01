📌 What is Git?



Git is a distributed version control system (DVCS) used to track changes in source code during software development.



🔹 Key Features

Tracks file changes over time

Supports branching and merging

Works offline

Enables collaboration among developers



👉 In simple terms: Git lets you save versions of your project and go back anytime.



🏗️ Git Architecture



Git works with a three-layer architecture:



1\. 🗂️ Working Directory

The actual project files on your system

Where you edit code

2\. 📦 Staging Area (Index)

Temporary area where you prepare changes before committing

Acts like a “preview” of your next commit

3\. 🗃️ Local Repository

Stores committed changes permanently

Contains full project history

🔁 Flow Diagram (Conceptual)

Working Directory → Staging Area → Local Repository

&#x20;     (edit)            (add)            (commit)

🌐 Remote Repository (Optional Layer)

Hosted on platforms like

GitHub,

GitLab

Used for sharing code with others

⚙️ Basic Git Commands



Here are the most commonly used commands:



🔹 Repository Setup

git init              # Initialize a new repo

git clone <url>       # Clone an existing repo

🔹 Tracking Changes

git status            # Check file status

git add <file>        # Add file to staging area

git add .             # Add all files

git commit -m "msg"   # Save changes

🔹 Viewing History

git log               # Show commit history

git diff              # Show changes

🔹 Branching

git branch            # List branches

git branch <name>     # Create branch

git checkout <name>   # Switch branch

git checkout -b <name> # Create + switch

🔹 Merging

git merge <branch>    # Merge branch into current

🔹 Remote Operations

git remote add origin <url>  # Add remote repo

git push origin main         # Push changes

git pull origin main         # Fetch + merge changes

🧠 Quick Summary

Git → tracks and manages code versions

Architecture → Working Directory → Staging → Repository

Commands → used to manage files, history, and collaboration

