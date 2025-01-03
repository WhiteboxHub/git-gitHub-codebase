## Working with Git Feature Branches

Below are some essential commands for handling feature branches in Git:

- **Create a new feature branch**:
    ```sh
    git checkout -b <feature-branch-name>
    ```

- **Switch to an existing feature branch**:
    ```sh
    git checkout <feature-branch-name>
    ```

- **List all branches, including feature branches**:
    ```sh
    git branch
    ```

- **Push the feature branch to the remote repository**:
    ```sh
    git push -u origin <feature-branch-name>
    ```

- **Merge the feature branch into the main branch**:
    ```sh
    git checkout main
    git merge <feature-branch-name>
    ```

- **Delete the feature branch locally**:
    ```sh
    git branch -d <feature-branch-name>
    ```

- **Delete the feature branch from the remote repository**:
    ```sh
    git push origin --delete <feature-branch-name>
    ```

- **Rebase the feature branch onto the main branch**:
    ```sh
    git checkout <feature-branch-name>
    git rebase main
    ```

- **View the commit history of the feature branch**:
    ```sh
    git log <feature-branch-name>
    ```

These commands are crucial for effectively managing feature branches in your Git repository.
