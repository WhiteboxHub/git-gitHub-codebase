Below are some essential commands for handling pull requests (PRs) in Git:

- **Create a new pull request**:
    1. Push your branch to the remote repository:
        ```sh
        git push -u origin <branch-name>
        ```
    2. Go to your repository on GitHub and click on "New pull request".

- **View existing pull requests**:
    ```sh
    git ls-remote --heads origin
    ```

- **Fetch and checkout a pull request locally**:
    ```sh
    git fetch origin pull/<PR-number>/head:<local-branch-name>
    git checkout <local-branch-name>
    ```

- **Merge a pull request**:
    1. Fetch the latest changes from the main branch:
        ```sh
        git checkout main
        git pull origin main
        ```
    2. Merge the pull request branch into the main branch:
        ```sh
        git merge <branch-name>
        ```
    3. Push the updated main branch to the remote repository:
        ```sh
        git push origin main
        ```

- **Close a pull request without merging**:
    1. Go to your repository on GitHub and navigate to the pull request.
    2. Click on "Close pull request".

These commands are crucial for effectively managing pull requests in your Git repository.
