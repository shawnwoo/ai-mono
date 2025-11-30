This is a monorepo for AI related projects.

Tech Stack:
Frontend: Next.js, React, TailwindCSS
Backend: Python, FastAPI
Local server start by using Tilt, Frontend server is using port 3000, Backend server is using port 8000
Both frontend and backend are using docker containers
For remote deployment, use Fly.io to deploy both frontend and backend containers

## Project Structure

```
.
├── apps
│   ├── web (Next.js, Port 3000)
│   └── api (FastAPI, Port 8000)
├── docker-compose.yml
├── Tiltfile
└── README.MD
```

## Getting Started

### Prerequisites
- Docker
- Tilt (optional, for `tilt up`)

### Running Locally

**Using Tilt:**
```bash
tilt up
```

**Using Docker Compose:**
```bash
docker-compose up --build
```

### Accessing Services
- **Frontend**: [http://localhost:3000](http://localhost:3000)
- **Backend**: [http://localhost:8000](http://localhost:8000)
- **Backend Docs**: [http://localhost:8000/docs](http://localhost:8000/docs)