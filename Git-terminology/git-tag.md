Below are some essential commands for handling tags in Git:

- **Create a new tag**:
    ```sh
    git tag <tag-name>
    ```

- **Create a new tag with a message**:
    ```sh
    git tag -a <tag-name> -m "tag message"
    ```

- **List all tags**:
    ```sh
    git tag
    ```

- **Show information about a specific tag**:
    ```sh
    git show <tag-name>
    ```

- **Delete a local tag**:
    ```sh
    git tag -d <tag-name>
    ```

- **Delete a remote tag**:
    ```sh
    git push origin --delete <tag-name>
    ```

- **Push a specific tag to the remote repository**:
    ```sh
    git push origin <tag-name>
    ```

- **Push all tags to the remote repository**:
    ```sh
    git push origin --tags
    ```

These commands are crucial for effectively managing tags in your Git repository.
