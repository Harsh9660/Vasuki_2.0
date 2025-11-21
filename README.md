# Vasuki 2.0

Vasuki 2.0 is a professional-grade chatbot application built with a modern tech stack.

## Tech Stack

- **Frontend**: React + Vite + Tailwind CSS
- **Backend**: Django + Django Rest Framework (Python)
- **Containerization**: Docker + Docker Compose

## Project Structure

```
Vasuki_2.0/
├── backend/                # Django Backend
│   ├── api/                # API App
│   ├── vasuki_backend/     # Project Settings
│   ├── Dockerfile          # Backend Dockerfile
│   └── requirements.txt    # Python Dependencies
├── src/                    # React Frontend Source
├── public/                 # Static Assets
├── Dockerfile              # Frontend Dockerfile
├── docker-compose.yml      # Docker Compose Configuration
└── package.json            # Node.js Dependencies
```

## Getting Started

### Prerequisites

- Docker and Docker Compose installed on your machine.

### Running the Application

1. **Clone the repository** (if applicable) or navigate to the project directory.

2. **Start the application using Docker Compose**:
   ```bash
   docker-compose up --build
   ```

3. **Access the Application**:
   - Frontend: [http://localhost:5173](http://localhost:5173)
   - Backend API: [http://localhost:8000](http://localhost:8000)

### Development

- **Frontend**: The frontend container supports hot module replacement (HMR). Changes in `src/` will be reflected immediately.
- **Backend**: The backend container mounts the code as a volume, so changes in `backend/` will trigger a server reload.

## API Endpoints

- `GET /api/health/`: Health check endpoint. Returns `{"status": "ok", "message": "Vasuki 2.0 Backend is running!"}`.
