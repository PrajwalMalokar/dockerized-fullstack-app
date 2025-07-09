# Dockerized Fullstack App

This project demonstrates a simple fullstack application with a Python backend and a Node.js/Express frontend, both containerized using Docker and orchestrated with Docker Compose.

## Features
- **Backend:** Python (Flask or similar)
- **Frontend:** Node.js with Express and EJS
- **Dockerized:** Each service has its own Dockerfile
- **Docker Compose:** Manages multi-container setup

## Project Structure
```
dockerized-fullstack-app/
    backend/        # Python backend service
    frontend/       # Node.js frontend service
    docker-compose.yaml
```

## Getting Started

### Prerequisites
- Docker
- Docker Compose

### Build and Run

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd dockerized-fullstack-app
   ```
2. Build and start the services:
   ```bash
   docker-compose up --build
   ```
3. Access the frontend at [http://localhost:3000](http://localhost:3000)
4. The backend API will be available at [http://localhost:8000/api](http://localhost:8000/api)

## Development
- Code changes in `backend/` or `frontend/` will reflect in the containers due to volume mounting.
- Update environment variables in `docker-compose.yaml` as needed.

## License
MIT
