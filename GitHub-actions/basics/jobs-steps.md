Below are some essential commands for handling `jobs and steps` in GitHub Actions:

- **Define a job in a workflow**:
    ```yaml
    jobs:
      example-job:
        runs-on: ubuntu-latest
        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Run a script
            run: echo "Hello, world!"
    ```

- **Define multiple jobs in a workflow**:
    ```yaml
    jobs:
      job1:
        runs-on: ubuntu-latest
        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Run a script
            run: echo "Job 1"
      job2:
        runs-on: ubuntu-latest
        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Run a script
            run: echo "Job 2"
    ```

- **Use job outputs in another job**:
    ```yaml
    jobs:
      job1:
        runs-on: ubuntu-latest
        steps:
          - name: Set output
            id: step1
            run: echo "::set-output name=example_output::Hello"
      job2:
        runs-on: ubuntu-latest
        needs: job1
        steps:
          - name: Use output from job1
            run: echo "Output from job1: ${{ steps.step1.outputs.example_output }}"
    ```

- **Define a matrix job**:
    ```yaml
    jobs:
      build:
        runs-on: ubuntu-latest
        strategy:
          matrix:
            node-version: [10, 12, 14]
        steps:
          - name: Checkout code
            uses: actions/checkout@v2
          - name: Setup Node.js
            uses: actions/setup-node@v2
            with:
              node-version: ${{ matrix.node-version }}
          - name: Install dependencies
            run: npm install
          - name: Run tests
            run: npm test
    ```

These commands are crucial for effectively managing jobs and steps in your GitHub Actions workflows.
