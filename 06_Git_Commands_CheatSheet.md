📘 Git Commands Cheat Sheet

🔹 Repository Setup

git init                     # Initialize new repo

git clone <url>              # Clone existing repo

🔹 Basic Workflow

git status                   # Check status

git add <file>               # Stage file

git add .                    # Stage all changes

git commit -m "message"      # Commit changes

🔹 Viewing Changes \& History

git log                      # Show commit history

git log --oneline            # Short log

git diff                     # Show unstaged changes

git show <commit>            # Show specific commit

🔹 Branching

git branch                   # List branches

git branch <name>            # Create branch

git checkout <branch>        # Switch branch

git checkout -b <branch>     # Create \& switch

git switch <branch>          # Modern switch command

🔹 Merging \& Rebase

git merge <branch>           # Merge branch

git rebase <branch>          # Rebase current branch

🔹 Remote Repositories

git remote add origin <url>  # Add remote

git remote -v                # View remotes

git push origin main         # Push to remote

git pull origin main         # Pull changes

git fetch                    # Fetch without merge

🔹 Undo Changes

git restore <file>           # Discard changes

git reset <file>             # Unstage file

git reset --hard             # Reset everything ⚠️

git revert <commit>          # Undo commit safely

🔹 Stashing

git stash                    # Save changes temporarily

git stash pop                # Reapply stash

git stash list               # List stashes

🔹 Tagging

git tag                      # List tags

git tag v1.0                 # Create tag

git push origin v1.0         # Push tag

🔹 Config

git config --global user.name "Your Name"

git config --global user.email "you@example.com"

git config --list

⚡ Pro Tips

Use Git aliases to shorten commands

Commit often with meaningful messages

Pull before pushing to avoid conflicts

Use branches for every feature

🧠 Ultra-Short Flow

git add → git commit → git push



