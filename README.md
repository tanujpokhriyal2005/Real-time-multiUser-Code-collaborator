# Multi-User Code Collaborator

A real-time collaborative code editor that allows multiple users to join a shared room, write code simultaneously, and communicate seamlessly.  
Built for developers, interview prep, pair programming, and collaborative learning.

## Features

- Real-time code synchronization across multiple users
- Create and join rooms using unique room IDs
- Multi-user collaborative editing
- Live typing updates using WebSockets
- Code execution support
- Language selection support
- Copy room ID functionality
- User join/leave notifications
- Responsive UI for desktop and mobile

## Tech Stack

### Frontend
- React.js
- Tailwind CSS
- Socket.IO Client

### Backend
- Node.js
- Express.js
- Socket.IO

### DevOps / Deployment
- Docker
- AWS

## How It Works

1. User creates a room or joins an existing room.
2. A unique room ID is generated.
3. Multiple users connect to the same room.
4. Code changes are broadcast instantly using WebSockets.
5. All connected users see live updates in real time.

