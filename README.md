
## DevOps Setup

This project runs on a React + Vite frontend, a .NET backend, an nginx reverse proxy, Docker Compose configuration, and a GitHub Actions CI/CD pipeline.

### Services

	- 'frontend': builds the React + Vite app and serves the static production output with Nginx.
	- 'backend': builds + runs the .NET backend API using a runtime-only container image.
	- 'nginx': acts as the public reverse proxy. It routes '/' to the frontend and '/api/' to the backend.

### Local Run Instructions

From the repository root, run:

docker compose up --build -d
