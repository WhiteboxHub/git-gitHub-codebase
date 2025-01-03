Below are some essential commands for handling `Docker` in GitHub Actions:

- **Build and push a Docker image**:
    ```yaml
    name: Build and push Docker image

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

          - name: Log in to Docker Hub
            run: echo "${{ secrets.DOCKER_PASSWORD }}" | docker login -u "${{ secrets.DOCKER_USERNAME }}" --password-stdin

          - name: Build Docker image
            run: docker build . -t my-image:latest

          - name: Push Docker image
            run: docker push my-image:latest
    ```

- **Run a Docker container**:
    ```yaml
    name: Run Docker container

    on:
      push:
        branches:
          - main

    jobs:
      run:
        runs-on: ubuntu-latest

        steps:
          - name: Checkout code
            uses: actions/checkout@v2

          - name: Run Docker container
            run: docker run my-image:latest
    ```

These commands are crucial for effectively managing Docker in your GitHub Actions workflows.
