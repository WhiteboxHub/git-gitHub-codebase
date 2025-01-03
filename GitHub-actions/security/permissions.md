Below are some essential commands for handling `Permissions` in GitHub Actions:

- **Set job permissions**:
    ```yaml
    name: Set job permissions

    on:
      push:
        branches:
          - main

    jobs:
      job1:
        runs-on: ubuntu-latest
        permissions:
          contents: read
          issues: write
        steps:
          - name: Checkout code
            uses: actions/checkout@v2

          - name: Run a script
            run: echo "Running with specific permissions"
    ```

- **Set workflow permissions**:
    ```yaml
    name: Set workflow permissions

    on:
      push:
        branches:
          - main

    permissions:
      contents: read
      issues: write

    jobs:
      job1:
        runs-on: ubuntu-latest
        steps:
          - name: Checkout code
            uses: actions/checkout@v2

          - name: Run a script
            run: echo "Running with workflow permissions"
    ```

These commands are crucial for effectively managing permissions in your GitHub Actions workflows.
