Below are some essential commands for handling `events and triggers` in GitHub Actions:

- **Trigger a workflow on push**:
    ```yaml
    name: CI

    on: 
      push:
        branches:
          - main

    jobs:
      build:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Run a script
            run: echo "Hello, world!"
    ```

- **Trigger a workflow on pull request**:
    ```yaml
    name: CI

    on: 
      pull_request:
        branches:
          - main

    jobs:
      build:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Run a script
            run: echo "Hello, world!"
    ```

- **Trigger a workflow on a schedule**:
    ```yaml
    name: Scheduled workflow

    on:
      schedule:
        - cron: '0 0 * * *'

    jobs:
      build:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Run a script
            run: echo "Hello, world!"
    ```

- **Trigger a workflow on repository dispatch**:
    ```yaml
    name: Repository dispatch

    on:
      repository_dispatch:
        types: [custom-event]

    jobs:
      build:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Run a script
            run: echo "Hello, world!"
    ```

These commands are crucial for effectively managing events and triggers in your GitHub Actions workflows.
