Below are some essential commands for handling `Secrets Management` in GitHub Actions:

- **Create and use secrets**:
    ```yaml
    name: Create and Use Secrets

    on:
      push:
        branches:
          - main

    jobs:
      secrets:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2

          - name: Use secret in a script
            run: echo "Your secret is ${{ secrets.YOUR_SECRET }}"
    ```

- **Use secrets in environment variables**:
    ```yaml
    name: Use Secrets in Environment Variables

    on:
      push:
        branches:
          - main

    jobs:
      secrets:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2

          - name: Use secret in environment variable
            run: echo "Your secret is $SECRET"
            env:
              SECRET: ${{ secrets.YOUR_SECRET }}
    ```

These commands are crucial for effectively managing secrets in your GitHub Actions workflows.
