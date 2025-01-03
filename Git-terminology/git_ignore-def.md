Below are some essential commands for handling `.gitignore` in Git:

- **Create or edit a `.gitignore` file**:
    ```sh
    nano .gitignore
    ```

- **Add a file or directory to `.gitignore`**:
    ```sh
    echo <file-or-directory-name> >> .gitignore
    ```

- **Check if a file is being ignored**:
    ```sh
    git check-ignore -v <file-name>
    ```

- **Apply changes in `.gitignore` to the repository**:
    ```sh
    git rm -r --cached .
    git add .
    git commit -m "Apply .gitignore changes"
    ```

These commands are crucial for effectively managing ignored files in your Git repository with `.gitignore`.

Below are some essential commands for handling `git diff` in Git:

- **Show changes between the working directory and the index**:
    ```sh
    git diff
    ```

- **Show changes between the index and the last commit**:
    ```sh
    git diff --cached
    ```

- **Show changes between two commits**:
    ```sh
    git diff <commit-hash-1> <commit-hash-2>
    ```

- **Show changes for a specific file**:
    ```sh
    git diff <commit-hash-1> <commit-hash-2> -- <file-name>
    ```

- **Show changes between the working directory and a specific commit**:
    ```sh
    git diff <commit-hash>
    ```

These commands are crucial for effectively managing differences in your Git repository with `git diff`.
