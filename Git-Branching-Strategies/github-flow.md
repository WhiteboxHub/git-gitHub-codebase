Below are some essential commands for handling `GitHub flow` in Git:

- **Create a new branch**:
    ```sh
    git checkout -b <branch-name>
    ```

- **Make changes and commit**:
    ```sh
    git add .
    git commit -m "Commit message"
    ```

- **Push the branch to GitHub**:
    ```sh
    git push origin <branch-name>
    ```

- **Create a pull request**:
    1. Go to your repository on GitHub.
    2. Click the "Compare & pull request" button next to your branch.
    3. Review the changes and submit the pull request.

- **Merge the pull request**:
    1. Once the pull request is approved, click the "Merge pull request" button.
    2. Confirm the merge.

- **Delete the branch**:
    ```sh
    git branch -d <branch-name>
    git push origin --delete <branch-name>
    ```

These commands are crucial for effectively managing your Git repository with `GitHub flow`.
