Below are some essential commands for handling `git reset` in Git:

- **Unstage a file**:
    ```sh
    git reset <file-name>
    ```

- **Soft reset to a specific commit (keeps changes in working directory)**:
    ```sh
    git reset --soft <commit-hash>
    ```

- **Mixed reset to a specific commit (keeps changes in working directory, unstages changes)**:
    ```sh
    git reset --mixed <commit-hash>
    ```

- **Hard reset to a specific commit (discards all changes)**:
    ```sh
    git reset --hard <commit-hash>
    ```

- **Reset a specific file to a specific commit**:
    ```sh
    git reset <commit-hash> <file-name>
    ```

These commands are crucial for effectively managing your Git repository with `git reset`.
