Below are some essential commands for handling forks in Git:

- **Fork a repository**:
    1. Go to the repository on GitHub you want to fork.
    2. Click the "Fork" button in the upper right corner.

- **Clone your forked repository**:
    ```sh
    git clone <your-forked-repo-url>
    ```

- **Add the original repository as a remote**:
    ```sh
    git remote add upstream <original-repo-url>
    ```

- **Fetch changes from the original repository**:
    ```sh
    git fetch upstream
    ```

- **Merge changes from the original repository into your fork**:
    ```sh
    git merge upstream/main
    ```

- **Push changes to your forked repository**:
    ```sh
    git push origin main
    ```

These commands are crucial for effectively managing your forked repositories in Git.
