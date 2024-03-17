# PLPBasicGitAssignment

This repository is a part of an assignment to familiarize students with the basic workflow of creating a GitHub repository, connecting it to a local folder, and making commits and pushes.

## Steps Followed

1. Created a new repository named "PLPBasicGitAssignment" on GitHub and initialized it with a README file.
2. Created a new folder named "PLPBasicGitAssignment" on the local machine.
3. Initialized a new Git repository in the local folder using the command: `git init`
4. Linked the local repository to the GitHub repository using the command: `git remote add origin <repository-url>`
5. Created a new text file named `hello.txt` in the local folder and added the text "Hello, Git!".
6. Staged the changes using the command: `git add hello.txt`
7. Committed the changes using the command: `git commit -m "Add hello.txt with a greeting"`

### Issue Encountered

While trying to push the committed changes to the GitHub repository, there was an issue because the local branch was named "master" while the remote branch was named "main". To resolve this, the following steps were taken:

1. Renamed the local branch from "master" to "main" using the command: `git branch -m master main`
2. Pulled the remote changes and allowed unrelated histories using the command: `git pull origin main --allow-unrelated-histories`
3. Finally, pushed the local changes to the GitHub repository using the command: `git push -u origin main`

## Verification

After executing the push command, the `hello.txt` file and commit message were successfully visible on the GitHub repository.