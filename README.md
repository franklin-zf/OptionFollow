# OptionFollow - 美股期权异动监控平台

This is the main repository for the OptionFollow project.

## Project Structure

- `/backend`: Contains the Python FastAPI backend application.
- `/frontend`: Contains the React (Vite) frontend application.

## Development Setup

This project is fully containerized using Docker. Make sure you have Docker and Docker Compose installed on your system.

### Running the Application

To start the entire application stack (backend, frontend, database, and Redis), run the following command from the project root:

```bash
docker-compose up --build
```

This command will:
1.  Build the Docker images for the backend and frontend services if they don't exist.
2.  Start all the services defined in `docker-compose.yml`.
3.  Mount the local code directories into the containers, so any changes you make will be reflected in real-time.

### Accessing the Services

Once the containers are up and running, you can access the services at the following URLs:

- **Backend API**: [http://localhost:8000](http://localhost:8000)
- **Frontend Application**: [http://localhost:5173](http://localhost:5173)
- **PostgreSQL Database**: Connect on port `5432` (credentials are in `docker-compose.yml`)
- **Redis**: Connect on port `6379`
