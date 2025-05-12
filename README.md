# Task Tracker Application

A full-stack task tracking application built with Express.js, React, and MongoDB.

## Features

- User authentication (signup/login)
- Project management (create, read, update, delete)
- Task management within projects
- Task status tracking
- Responsive Material-UI design

## Tech Stack

### Backend
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- Express Validator

### Frontend
- React with TypeScript
- Material-UI
- React Router
- Axios

## Prerequisites

- Node.js (v14 or higher)
- MongoDB
- npm or yarn

## Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd task-tracker
```

2. Install backend dependencies:
```bash
cd backend
npm install
```

3. Create a `.env` file in the backend directory:
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/task-tracker
JWT_SECRET=your-secret-key
```

4. Install frontend dependencies:
```bash
cd ../frontend
npm install
```

5. Start the backend server:
```bash
cd ../backend
npm run dev
```

6. Start the frontend development server:
```bash
cd ../frontend
npm start
```

The application will be available at:
- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## API Endpoints

### Authentication
- POST /api/auth/register - Register a new user
- POST /api/auth/login - Login user

### Projects
- GET /api/projects - Get all projects
- POST /api/projects - Create a new project
- GET /api/projects/:id - Get a single project
- PUT /api/projects/:id - Update a project
- DELETE /api/projects/:id - Delete a project

### Tasks
- GET /api/tasks - Get all tasks
- POST /api/tasks - Create a new task
- GET /api/tasks/:id - Get a single task
- PUT /api/tasks/:id - Update a task
- DELETE /api/tasks/:id - Delete a task

## Project Structure

```
task-tracker/
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── middleware/
│   │   └── config/
│   └── package.json
└── frontend/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── services/
    │   ├── types/
    │   └── utils/
    └── package.json
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License. 