Below are some essential commands for handling `Node.js` in GitHub Actions:

- **Setup Node.js environment**:
    ```yaml
    name: Setup Node.js environment

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

          - name: Setup Node.js
            uses: actions/setup-node@v2
            with:
              node-version: '14'
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

          - name: Setup Node.js
            uses: actions/setup-node@v2
            with:
              node-version: '14'

          - name: Install dependencies
            run: npm install

          - name: Run tests
            run: npm test
    ```

These commands are crucial for effectively managing Node.js in your GitHub Actions workflows.
