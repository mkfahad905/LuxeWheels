# LuxeWheels

A premium full-stack e-commerce platform designed for browsing, buying, and renting luxury pre-owned cars. LuxeWheels provides a seamless user experience backed by a robust RESTful API and a modern React frontend.

## Features

- **User Authentication**: Secure JWT-based authentication and authorization for user sessions.
- **Administrative Dashboard**: A dedicated interface for administrators.
- **Responsive Design**: Optimized for both desktop and mobile viewing experiences.

## Tech Stack

LuxeWheels is built using the **MERN** stack:

### Backend
- **Node.js & Express**: High-performance REST API routing.
- **MongoDB & Mongoose**: Flexible NoSQL database and schema modeling.
- **JWT & bcryptjs**: Security and password hashing.

### Frontend
- **React 19 (Vite)**: Modern, fast frontend framework.
- **React Router**: Client-side routing.
- **Axios**: HTTP client for API communication.

## Project Structure

The repository is divided into two main environments:

- `/backend/`: Contains the Express server, Mongoose models, controllers, middleware, and routing logic.
- `/frontend/LuxeWheels/`: Contains the Vite/React application, UI components, pages, and API service handlers.

## Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB (Local or Atlas)

### Environment Variables
Create a `.env` file in the `/backend/` directory with the following variables:
```env
JWT_SECRET=your_jwt_secret_key
PORT=5000
```

*Note: The MongoDB connection string is currently hardcoded in `backend/model/db.js` as `mongodb://localhost:27017/LuxeWheels`. Ensure you have a local MongoDB instance running on this default port.*

### Running the Backend
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```

### Running the Frontend
1. Navigate to the frontend directory:
   ```bash
   cd frontend/LuxeWheels
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the Vite development server:
   ```bash
   npm run dev
   ```

## Screenshots

*(Developers: Add high-quality screenshots of the platform here to demonstrate the UI/UX)*
