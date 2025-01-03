Below are some essential commands for handling hotfix branches in Git:

- **Create a new hotfix branch**:
    ```sh
    git checkout -b <hotfix-branch-name>
    ```

- **Switch to an existing hotfix branch**:
    ```sh
    git checkout <hotfix-branch-name>
    ```

- **List all branches, including hotfix branches**:
    ```sh
    git branch
    ```

- **Push the hotfix branch to the remote repository**:
    ```sh
    git push -u origin <hotfix-branch-name>
    ```

- **Merge the hotfix branch into the main branch**:
    ```sh
    git checkout main
    git merge <hotfix-branch-name>
    ```

- **Delete the hotfix branch locally**:
    ```sh
    git branch -d <hotfix-branch-name>
    ```

- **Delete the hotfix branch from the remote repository**:
    ```sh
    git push origin --delete <hotfix-branch-name>
    ```

- **Rebase the hotfix branch onto the main branch**:
    ```sh
    git checkout <hotfix-branch-name>
    git rebase main
    ```

- **View the commit history of the hotfix branch**:
    ```sh
    git log <hotfix-branch-name>
    ```

These commands are crucial for effectively managing hotfix branches in your Git repository.
