🌿 What is Branching?



In Git, branching means creating a separate line of development from the main codebase.



👉 It allows you to:



Work on features independently

Fix bugs without affecting main code

Experiment safely



By default, Git has a main branch (usually main or master).



📂 Types of Branches

🔹 1. Main (Master) Branch

The primary branch

Contains stable, production-ready code

🔹 2. Feature Branch

Used to develop new features

Created from main and merged back after completion



👉 Example:



git checkout -b feature-login

🔹 3. Bugfix Branch

Created to fix bugs

Usually branched from main or develop

🔹 4. Release Branch

Prepared for a new production release

Used for final testing and minor fixes

🔹 5. Hotfix Branch

Urgent fixes for production issues

Created directly from main

🌟 Popular Branching Strategies

🔹 1. Git Flow



A structured and widely used model.



📌 Branches:

main → production

develop → ongoing development

feature, release, hotfix branches



👉 Flow:



feature → develop → release → main



✔ Best for large projects with planned releases



🔹 2. GitHub Flow



Simple and lightweight (used with GitHub)



📌 Steps:

Create branch

Make changes

Open Pull Request

Review \& merge



✔ Best for continuous deployment



🔹 3. GitLab Flow



Used with GitLab



Combines feature branches + environment branches

Supports CI/CD integration



✔ Good for DevOps workflows



🔹 4. Trunk-Based Development

Work mostly on a single branch (main)

Short-lived branches



✔ Best for fast-moving teams \& CI/CD



⚖️ Quick Comparison

Strategy	Complexity	Best For

Git Flow	High	Large projects

GitHub Flow	Low	Web apps, startups

GitLab Flow	Medium	DevOps teams

Trunk-Based	Low	Continuous delivery

🧠 Summary

Branching → parallel development in Git

Types → main, feature, bugfix, release, hotfix

Strategies → Git Flow, GitHub Flow, GitLab Flow, Trunk-based

