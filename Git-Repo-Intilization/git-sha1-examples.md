## Working with Git SHA-1 Hashes

Below are some essential commands for handling SHA-1 hashes in Git:

- **Display the commit history with abbreviated SHA-1 hashes**:
    ```sh
    git log --oneline
    ```

- **View details of a specific commit using its SHA-1 hash**:
    ```sh
    git show <commit-SHA-1>
    ```

- **Switch to a specific commit using its SHA-1 hash**:
    ```sh
    git checkout <commit-SHA-1>
    ```

- **Undo changes to a specific commit using its SHA-1 hash**:
    ```sh
    git revert <commit-SHA-1>
    ```

- **Return to a specific commit using its SHA-1 hash**:
    ```sh
    git reset --hard <commit-SHA-1>
    ```

- **Apply changes from a specific commit using its SHA-1 hash**:
    ```sh
    git cherry-pick <commit-SHA-1>
    ```

- **Retrieve the SHA-1 hash of the latest commit**:
    ```sh
    git rev-parse HEAD
    ```

- **Get the SHA-1 hash of a specific branch or tag**:
    ```sh
    git rev-parse <branch-or-tag-name>
    ```

These commands are crucial for effectively managing SHA-1 hashes in your Git repository.
