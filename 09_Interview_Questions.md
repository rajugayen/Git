🔹 Basic Git Questions



1\. What is Git and why is it used?

Answer: Git is a distributed version control system (DVCS) used to track changes in files, collaborate with multiple developers, and manage project history efficiently. It allows branching, merging, and offline work.



2\. Difference between Git and GitHub?

Answer:



Git – A version control system installed locally for tracking changes.

GitHub – A cloud platform for hosting Git repositories, enabling collaboration, pull requests, and CI/CD integration.



3\. What is a commit in Git?

Answer: A commit is a snapshot of your staged changes, stored in the local repository. Each commit has a unique ID (hash) and a message describing the changes.



4\. How do you revert a commit?

Answer:



git revert <commit> – Creates a new commit that undoes the changes (safe for shared repos).

git reset --hard <commit> – Moves branch pointer back, discarding commits (not safe for shared repos).



5\. Difference between git pull and git fetch?

Answer:



git fetch – Downloads changes from remote without merging.

git pull – Downloads and merges changes into your current branch.



6\. Explain the staging area in Git.

Answer: The staging area (index) is a buffer between working directory and local repository where you prepare changes before committing.



7\. How do you undo changes in Git?

Answer:



git restore <file> – Undo uncommitted changes.

git reset <file> – Unstage a file.

git checkout <commit> <file> – Restore from a previous commit.

🔹 Branching \& Merging



1\. What is a branch in Git?

Answer: A branch is a parallel line of development that allows you to work on features or fixes independently of the main code.



2\. Different types of branches?

Answer:



Main/Master – Stable production-ready code.

Feature branch – For developing new features.

Bugfix branch – For resolving issues.

Release branch – For preparing a release.

Hotfix branch – For urgent production fixes.



3\. What is a merge conflict and how do you resolve it?

Answer: A merge conflict happens when Git cannot automatically combine changes (e.g., same line edited in two branches).

Resolution steps:



Identify conflicted files: git status

Manually fix conflicts

Stage the file: git add <file>

Commit merge: git commit



4\. Difference between merge and rebase?

Answer:



Merge – Combines branches with a merge commit.

Rebase – Moves commits from one branch on top of another, creating a linear history.



5\. Branching strategies?

Answer:



Git Flow – Structured (main, develop, feature, release, hotfix)

GitHub Flow – Lightweight; feature → PR → merge → deploy

GitLab Flow – Feature branches + environment branches with CI/CD

Trunk-Based – Single main branch; short-lived branches

🔹 Remote Repositories \& Collaboration



1\. How do you clone a repository?

Answer:



git clone <repository-url>



2\. How do you push changes to remote?

Answer:



git push origin <branch>



3\. Explain pull requests (PRs) and code reviews.

Answer: A PR is a request to merge your branch into another (usually main). Team members review code, run tests, and approve before merging.



4\. How do you handle someone else’s changes in your branch?

Answer: Pull latest changes and merge/rebase:



git pull origin main

\# OR for linear history

git fetch origin

git rebase origin/main



5\. Difference between origin and upstream?

Answer:



origin – Your fork’s remote repository

upstream – Original repository you forked from

🔹 CI/CD \& DevOps Integration



1\. What is CI/CD and why is it important?

Answer:



CI (Continuous Integration) – Automatically build and test code on every push.

CD (Continuous Delivery/Deployment) – Automatically release or deploy code.

Importance: Faster, safer, and automated delivery.



2\. How does Git integrate with CI/CD pipelines?

Answer: Git triggers pipelines whenever changes are pushed. CI/CD tools like GitHub Actions, GitLab CI, Jenkins detect the push, build, test, and deploy code.



3\. Real-world CI/CD scenario?



Developer creates a feature branch → push → PR → CI pipeline runs tests → merge → CD deploys to staging/production.



4\. What happens if a build fails in CI/CD?

Answer: The pipeline stops, the developer is notified, and the failed commit is not deployed until fixed.



5\. How do hotfixes get deployed?

Answer: Create a hotfix branch from main, fix the bug, push, CI/CD runs fast-track tests, then merge back into main and other branches.



🔹 Advanced Git Questions



1\. Difference between Git and SVN?

Answer:



Git – Distributed VCS, full repo on each machine, offline work.

SVN – Centralized VCS, relies on a single server, limited offline work.



2\. Git tags?

Answer: Tags mark important commits like releases:



git tag v1.0

git push origin v1.0



3\. Git stash?

Answer: Temporarily saves uncommitted changes:



git stash

git stash pop



4\. Difference between git reset, git revert, git checkout?



reset – Moves branch pointer, can discard commits

revert – Safe undo by creating a new commit

checkout – Switch branches or restore files



5\. Git hooks?

Answer: Scripts that run on events (commit, push).

Example: pre-commit hook to run linting automatically.



🔹 Scenario-Based Questions



1\. Conflicting changes pushed by another developer?



Pull latest changes → merge/rebase → resolve conflicts → commit → push



2\. Production critical bug?



Create hotfix branch → fix bug → push → run CI/CD → deploy → merge back into develop



3\. Release a new version safely?



Use release branch → test → tag → merge into main → deploy



4\. Clean Git history before merging?



Use interactive rebase:

git rebase -i HEAD\~5



5\. Tricky merge conflict experience?



Example answer: “I resolved a conflict by manually merging the conflicting lines, testing locally, then pushing the resolved branch and informing the team.”

⚡ Interview Tips

Always mention Git commands and workflows.

Give real examples from your experience.

Structure answers: Definition → Command/Example → Best Practices.

Highlight CI/CD integration if relevant.



