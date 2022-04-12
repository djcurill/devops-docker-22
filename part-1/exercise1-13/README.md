# Exercise
Clone, fork or download a project from https://github.com/docker-hy/material-applications/tree/main/example-backend.

Create a Dockerfile for the project (example-backend). Start the container with port 8080 published.

When you start the container and navigate to http://localhost:8080/ping you should get a "pong" as response.

Submit the Dockerfile and the command used.

# Solution
See dockerfile.

Command:
```bash
cd /path/to/example-backend-repo
docker build -t example-backend .
docker run --rm --name go-service -p 3000:8080 example-backend
```