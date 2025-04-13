# Modern CMS Project

A full-stack Content Management System built with Go, React, and modern web technologies.

## Tech Stack

### Backend
- Go (Gin framework)
- PostgreSQL (Main database)
- MongoDB (Content storage)
- JWT Authentication
- Role-based access control

### Frontend
- React
- TailwindCSS
- React Router
- Axios

## Project Structure
```
.
├── backend/           # Go backend application
├── frontend/         # React frontend application
└── docker/           # Docker configuration files
```

## Getting Started

### Prerequisites
- Go 1.21 or higher
- Node.js 18 or higher
- PostgreSQL 15 or higher
- MongoDB 6 or higher
- Docker (optional)

### Development Setup

1. Clone the repository
2. Set up the backend:
   ```bash
   cd backend
   go mod download
   go run main.go
   ```

3. Set up the frontend:
   ```bash
   cd frontend
   npm install
   npm run dev
   ```

4. Set up databases:
   - PostgreSQL: Create a database named `cms_db`
   - MongoDB: Create a database named `cms_content`

## Environment Variables

Create `.env` files in both backend and frontend directories with the following variables:

### Backend (.env)
```
DB_HOST=localhost
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=your_password
DB_NAME=cms_db
MONGODB_URI=mongodb://localhost:27017
JWT_SECRET=your_jwt_secret
```

### Frontend (.env)
```
VITE_API_URL=http://localhost:8080
```

## License
MIT 