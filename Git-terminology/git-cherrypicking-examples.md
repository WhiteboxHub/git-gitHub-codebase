Below are some essential commands for handling cherry-picking in Git:

- **Cherry-pick a commit**:
    ```sh
    git cherry-pick <commit-hash>
    ```

- **Continue cherry-picking after resolving conflicts**:
    ```sh
    git cherry-pick --continue
    ```

- **Skip the current commit during a cherry-pick**:
    ```sh
    git cherry-pick --skip
    ```

- **Abort a cherry-pick in progress**:
    ```sh
    git cherry-pick --abort
    ```

- **Cherry-pick a range of commits**:
    ```sh
    git cherry-pick <start-commit-hash>^..<end-commit-hash>
    ```

- **Cherry-pick multiple non-sequential commits**:
    ```sh
    git cherry-pick <commit-hash-1> <commit-hash-2> <commit-hash-3>
    ```

These commands are crucial for effectively managing cherry-picking in your Git repository.
