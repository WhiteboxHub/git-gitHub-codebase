## Working with Git SSH

Below are some essential commands for handling SSH in Git:

- **Generate a new SSH key**:
    ```sh
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```

- **Start the SSH agent in the background**:
    ```sh
    eval "$(ssh-agent -s)"
    ```

- **Add your SSH private key to the SSH agent**:
    ```sh
    ssh-add ~/.ssh/id_rsa
    ```

- **Add the SSH key to your GitHub account**:
    1. Copy the SSH key to your clipboard:
        ```sh
        cat ~/.ssh/id_rsa.pub
        ```
    2. Go to GitHub, navigate to **Settings** > **SSH and GPG keys** > **New SSH key**, and paste the key.

- **Test your SSH connection to GitHub**:
    ```sh
    ssh -T git@github.com
    ```

- **Clone a repository using SSH**:
    ```sh
    git clone git@github.com:username/repository.git
    ```

- **Add a remote repository using SSH**:
    ```sh
    git remote add origin git@github.com:username/repository.git
    ```

- **Push changes to the remote repository using SSH**:
    ```sh
    git push -u origin master
    ```

These commands are crucial for effectively managing SSH keys and connections in your Git repository.
