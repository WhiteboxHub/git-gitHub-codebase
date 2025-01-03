Below are some essential commands for handling stashing in Git:

- **Stash changes**:
    ```sh
    git stash
    ```

- **Apply the latest stash**:
    ```sh
    git stash apply
    ```

- **Apply a specific stash**:
    ```sh
    git stash apply stash@{<stash-number>}
    ```

- **List all stashes**:
    ```sh
    git stash list
    ```

- **Drop a specific stash**:
    ```sh
    git stash drop stash@{<stash-number>}
    ```

- **Clear all stashes**:
    ```sh
    git stash clear
    ```

These commands are crucial for effectively managing your Git repository with `git stash`.
