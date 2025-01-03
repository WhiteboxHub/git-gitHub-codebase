Below are some essential commands for handling `GitLab flow` in Git:

- **Create a new branch**:
    ```sh
    git checkout -b <branch-name>
    ```

- **Make changes and commit**:
    ```sh
    git add .
    git commit -m "Commit message"
    ```

- **Push the branch to GitLab**:
    ```sh
    git push origin <branch-name>
    ```

- **Create a merge request**:
    1. Go to your repository on GitLab.
    2. Click the "Merge Requests" tab.
    3. Click the "New merge request" button.
    4. Select the source and target branches, then click "Compare branches and continue".
    5. Fill in the details and submit the merge request.

- **Merge the merge request**:
    1. Once the merge request is approved, click the "Merge" button.
    2. Confirm the merge.

- **Delete the branch**:
    ```sh
    git branch -d <branch-name>
    git push origin --delete <branch-name>
    ```

These commands are crucial for effectively managing your Git repository with `GitLab flow`.
