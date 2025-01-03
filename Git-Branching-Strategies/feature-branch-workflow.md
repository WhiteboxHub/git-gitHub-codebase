Below are some essential commands for handling `feature branch workflow` in Git:

- **Create a new feature branch**:
    ```sh
    git checkout -b <feature-branch-name>
    ```

- **Make changes and commit**:
    ```sh
    git add .
    git commit -m "Commit message"
    ```

- **Push the feature branch to the remote repository**:
    ```sh
    git push origin <feature-branch-name>
    ```

- **Create a pull request**:
    1. Go to your repository on the remote platform (e.g., GitHub, GitLab).
    2. Click the "Compare & pull request" button next to your branch.
    3. Review the changes and submit the pull request.

- **Merge the pull request**:
    1. Once the pull request is approved, click the "Merge pull request" button.
    2. Confirm the merge.

- **Delete the feature branch**:
    ```sh
    git branch -d <feature-branch-name>
    git push origin --delete <feature-branch-name>
    ```

These commands are crucial for effectively managing your Git repository with `feature branch workflow`.
