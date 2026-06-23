# MultiCodeCollaborator

## Deployed Link

- http://54.95.0.72:3000

## Project Overview

MultiCodeCollaborator is a collaborative code editing web app built with a React frontend and an Express backend. Users can join with a username, share a live Monaco-based code editor, and see other connected collaborators in real time.

The frontend connects to the backend via Socket.IO and Yjs awareness, so text changes and presence are synchronized instantly across all users.

## Key Features

- Real-time collaborative code editing
- Multi-user presence list with active usernames
- Monaco editor integration for code editing experience
- Backend health route and static file serving
- Docker-ready build for deployment

## Tech Stack

- Frontend:
  - React
  - Vite
  - Tailwind CSS
  - @monaco-editor/react
  - Yjs
  - y-socket.io
  - y-monaco

- Backend:
  - Node.js
  - Express
  - Socket.IO
  - Y-socket.io

- Deployment / DevOps:
  - Docker
  - AWS-hosted container deployment

## Repo Structure

- `Frontend/` - React client application
- `Backend/` - Node/Express server and Socket.IO collaboration backend
- `dockerfile` - multi-stage Docker build that builds the frontend and serves it from the backend

## How to Run Locally

### Backend

```bash
cd Backend
npm install
npm run dev
```

### Frontend

```bash
cd Frontend
npm install
npm run dev
```

### Docker

Build and run the Docker image from the repository root:

```bash
docker build -t multicodecollaborator .
docker run -p 3000:3000 multicodecollaborator
```

Then open:

- http://localhost:3000

## Notes

- The deployed AWS app is available at `http://54.95.0.72:3000`.
- The backend serves the built frontend from `Backend/public` when running inside Docker.
- The app supports collaborative editing and user awareness via Yjs and Socket.IO.
