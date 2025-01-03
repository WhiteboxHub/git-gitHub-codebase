Below are some essential commands for handling `git revert` in Git:

- **Revert a specific commit**:
    ```sh
    git revert <commit-hash>
    ```

- **Revert multiple commits**:
    ```sh
    git revert <oldest-commit-hash>^..<newest-commit-hash>
    ```

- **Revert a range of commits interactively**:
    ```sh
    git revert -n <oldest-commit-hash>^..<newest-commit-hash>
    ```

- **Abort a revert operation**:
    ```sh
    git revert --abort
    ```

These commands are crucial for effectively managing your Git repository with `git revert`.
