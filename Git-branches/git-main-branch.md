## Working with the Git Main Branch

Below are some essential commands and information for handling the main branch in Git:

- **Create a new main branch**:
    ```sh
    git branch main
    ```

- **Switch to the main branch**:
    ```sh
    git checkout main
    ```

- **Rename the current branch to main**:
    ```sh
    git branch -m main
    ```

- **Push the main branch to the remote repository**:
    ```sh
    git push -u origin main
    ```

- **Set the upstream branch for the main branch**:
    ```sh
    git branch --set-upstream-to=origin/main main
    ```

- **Merge another branch into the main branch**:
    ```sh
    git checkout main
    git merge <branch-name>
    ```

- **Delete the main branch locally**:
    ```sh
    git branch -d main
    ```

- **Delete the main branch from the remote repository**:
    ```sh
    git push origin --delete main
    ```

- **Rebase the main branch onto another branch**:
    ```sh
    git checkout main
    git rebase <branch-name>
    ```

- **View the commit history of the main branch**:
    ```sh
    git log main
    ```

These commands are crucial for effectively managing the main branch in your Git repository.
