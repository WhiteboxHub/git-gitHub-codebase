Below are some essential commands and concepts for handling core Git functionalities:

- **HEAD**:
    - **View the current HEAD**:
        ```sh
        git rev-parse HEAD
        ```
    - **Move HEAD to a specific commit**:
        ```sh
        git reset --hard <commit-hash>
        ```

- **Index**:
    - **View the current index**:
        ```sh
        git ls-files -s
        ```
    - **Add changes to the index**:
        ```sh
        git add <file-name>
        ```

- **Fetch**:
    - **Fetch changes from the remote repository**:
        ```sh
        git fetch
        ```
    - **Fetch changes from a specific branch**:
        ```sh
        git fetch origin <branch-name>
        ```

- **Merge**:
    - **Merge a branch into the current branch**:
        ```sh
        git merge <branch-name>
        ```
    - **Abort a merge in progress**:
        ```sh
        git merge --abort
        ```

- **Origin**:
    - **View the remote repository URL**:
        ```sh
        git remote get-url origin
        ```
    - **Set a new remote repository URL**:
        ```sh
        git remote set-url origin <new-url>
        ```

These commands and concepts are crucial for effectively managing core functionalities in your Git repository.
