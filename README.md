## Project2

## Image Hosting

## Application for downloading and storing images in .jpg, .jpeg, .png, .gif formats

## The system consists of two main components:
- Python backend:
Responsible for processing HTTP requests, uploading images, validating data, and logging.
Executes the application's business logic related to managing uploaded files.
Works inside a Docker container, listening for requests on port 8000.

- Nginx server:
Serves static files and uploaded images via the /images/ route.
Proxies requests to the Python backend for other routes.
Runs in a separate Docker container, listening for requests on port 80.

The components communicate via a local network created using Docker Compose.

## Requirements:
- Docker
- Docker Compose
- Loguru

## Launch:
To launch the system, you need to:
- Install Docker and Docker Compose.
- Run the command: docker-compose up --build

## Stop and delete:
- To stop and delete, run the command: docker-compose down
