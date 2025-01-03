Below are some essential commands for handling release branches in Git:

- **Create a new release branch**:
    ```sh
    git checkout -b <release-branch-name>
    ```

- **Switch to an existing release branch**:
    ```sh
    git checkout <release-branch-name>
    ```

- **List all branches, including release branches**:
    ```sh
    git branch
    ```

- **Push the release branch to the remote repository**:
    ```sh
    git push -u origin <release-branch-name>
    ```

- **Merge the release branch into the main branch**:
    ```sh
    git checkout main
    git merge <release-branch-name>
    ```

- **Delete the release branch locally**:
    ```sh
    git branch -d <release-branch-name>
    ```

- **Delete the release branch from the remote repository**:
    ```sh
    git push origin --delete <release-branch-name>
    ```

- **Rebase the release branch onto the main branch**:
    ```sh
    git checkout <release-branch-name>
    git rebase main
    ```

- **View the commit history of the release branch**:
    ```sh
    git log <release-branch-name>
    ```

These commands are crucial for effectively managing release branches in your Git repository.
