Below are some essential commands for handling `Python` in GitHub Actions:

- **Setup Python environment**:
    ```yaml
    name: Setup Python environment

    on:
      push:
        branches:
          - main

    jobs:
      setup:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2

          - name: Setup Python
            uses: actions/setup-python@v2
            with:
              python-version: '3.8'
    ```

- **Install dependencies and run tests**:
    ```yaml
    name: Install dependencies and run tests

    on:
      push:
        branches:
          - main

    jobs:
      test:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2

          - name: Setup Python
            uses: actions/setup-python@v2
            with:
              python-version: '3.8'

          - name: Install dependencies
            run: pip install -r requirements.txt

          - name: Run tests
            run: pytest
    ```

These commands are crucial for effectively managing Python in your GitHub Actions workflows.
