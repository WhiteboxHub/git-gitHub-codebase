Below are some essential commands for handling `environment variables` in GitHub Actions:

- **Define an environment variable in a workflow**:
    ```yaml
    jobs:
      example-job:
        runs-on: ubuntu-latest
        env:
          EXAMPLE_VAR: 'example_value'
        steps:
          - name: Print environment variable
            run: echo $EXAMPLE_VAR
    ```

- **Define an environment variable for a specific step**:
    ```yaml
    jobs:
      example-job:
        runs-on: ubuntu-latest
        steps:
          - name: Set environment variable
            run: echo "EXAMPLE_VAR=example_value" >> $GITHUB_ENV
          - name: Print environment variable
            run: echo $EXAMPLE_VAR
    ```

- **Use secrets as environment variables**:
    ```yaml
    jobs:
      example-job:
        runs-on: ubuntu-latest
        steps:
          - name: Print secret
            env:
              SECRET_VAR: ${{ secrets.SECRET_NAME }}
            run: echo $SECRET_VAR
    ```

- **Persist environment variables between steps**:
    ```yaml
    jobs:
      example-job:
        runs-on: ubuntu-latest
        steps:
          - name: Set environment variable
            run: echo "EXAMPLE_VAR=example_value" >> $GITHUB_ENV
          - name: Print environment variable
            run: echo $EXAMPLE_VAR
    ```

These commands are crucial for effectively managing environment variables in your GitHub Actions workflows.
