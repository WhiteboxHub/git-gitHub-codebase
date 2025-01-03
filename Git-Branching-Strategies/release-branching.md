Below are some essential commands for handling `release branching` in Git:

- **Create a new release branch**:
    ```sh
    git checkout -b release/<release-name>
    ```

- **Make changes and commit**:
    ```sh
    git add .
    git commit -m "Commit message"
    ```

- **Push the release branch to the remote repository**:
    ```sh
    git push origin release/<release-name>
    ```

- **Merge the release branch into the main branch**:
    ```sh
    git checkout main
    git merge release/<release-name>
    ```

- **Tag the release**:
    ```sh
    git tag -a <tag-name> -m "Tag message"
    git push origin <tag-name>
    ```

- **Delete the release branch**:
    ```sh
    git branch -d release/<release-name>
    git push origin --delete release/<release-name>
    ```

These commands are crucial for effectively managing your Git repository with `release branching`.
