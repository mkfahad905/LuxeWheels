# LuxeWheels

A full-stack web application skeleton featuring a React frontend and an Express/MongoDB backend with JWT-based user authentication.

## Overview

LuxeWheels serves as a foundational boilerplate for a web application. It implements a decoupled client-server architecture, providing a user authentication flow utilizing JSON Web Tokens (JWT) and hashed passwords. 

## Features

- **User Registration and Login**: User authentication flow with password hashing and JWT-based authorization.
- **JWT Authorization**: Session management using JSON Web Tokens.
- **RESTful API**: Express-based backend API handling user data.

## Tech Stack

### Frontend
- React 19
- Vite
- React Router DOM
- Axios

### Backend
- Node.js
- Express

### Database
- MongoDB
- Mongoose

### Authentication / Security
- JSON Web Tokens (JWT)
- bcryptjs
- CORS

### Development Tools
- Nodemon
- ESLint

## Architecture

Frontend (React) &rarr; REST API (Axios) &rarr; Backend (Express) &rarr; Database (MongoDB)

## Project Structure

- `backend/`
  - `controllers/` — Request handling logic.
  - `middlewares/` — Validation and authentication middleware.
  - `model/` — Mongoose schemas and database connection.
  - `routes/` — Express API route definitions.
- `frontend/LuxeWheels/`
  - `src/`
    - `pages/` — React views (Home, Login, Register, Admin).

## Getting Started

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the backend server:
   ```bash
   npm run dev
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend/LuxeWheels
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

## Configuration

The backend server utilizes a `.env` file for configuration. Create a `.env` file in the `backend/` directory:

```env
PORT=3003
JWT_SECRET=your_secret_key
```

*Note: The MongoDB connection string is currently hardcoded in `backend/model/db.js` (`mongodb://localhost:27017/LuxeWheels`). It does not currently use an environment variable.*

## Development

- Backend development server (with Nodemon): `npm run dev`
- Frontend development server (Vite): `npm run dev`

## Notes

- **Implementation Status**: The application currently focuses solely on user authentication (Login/Register). Extended e-commerce features (such as browsing, buying, or renting vehicles) are not yet implemented.
- **Database Configuration**: Ensure you have a local MongoDB instance running on port `27017` before starting the backend, due to the hardcoded connection string.
