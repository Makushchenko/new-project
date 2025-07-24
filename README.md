# new-project Setup Guide

Follow these steps to set up your `new-project` repository:

1. **Create a new directory** named `new-project` in your environment.
2. **Navigate** to the `new-project` directory:

   ```bash
   cd new-project
   ```
3. **Initialize** a new **public** Git repository:

   ```bash
   git init
   ```
4. **Create** a new file named `README.md` and add some initial text.
5. **Stage** the `README.md` file for commit:

   ```bash
   git add README.md
   ```
6. **Commit** the changes with the message `init`:

   ```bash
   git commit -m "init"
   ```
7. **Add** the remote repository URL:

   ```bash
   git remote add origin https://github.com/<user_name>/new-project.git
   ```
8. **Push** the `main` branch to the remote repository:

   ```bash
   git push -u origin main
   ```
9. **Create** a new branch named `development` and **switch** to it:

   ```bash
   git checkout -b development
   ```
10. **Edit** the `README.md` file to add your new instructions.
11. **Stage** the updated `README.md` file:

    ```bash
    git add README.md
    ```
12. **Commit** the changes on the `development` branch using a Smart Commit message (see [Smart Commit commands](https://support.atlassian.com/jira-software-cloud/docs/process-issues-with-smart-commits/#Smart-Commit-commands)):

    ```bash
    git commit -m "PROM-42164 #comment Added development instructions #time 1h"
    ```
13. **Merge** the changes from `development` into `main`:

    ```bash
    git checkout main
    git merge development
    ```
14. **Check** the status to ensure everything is up to date:

    ```bash
    git status
    ```
15. **Commit** any remaining changes if needed:

    ```bash
    git add .
    git commit -m "chore: finalize setup"
    ```