# Real-Time Quiz Application

A full-stack, real-time interactive Quiz application built with **Next.js** for the frontend and **Node.js/Express** for the backend. It leverages **Socket.IO** for live, real-time interactions (e.g., live quiz participation).

## 🚀 Features

- **Real-Time Interactions**: Powered by Socket.IO for live quiz sessions.
- **User Authentication**: Secure login and registration using JWT and Bcrypt.
- **Interactive UI**: Built with Next.js 15, React 19, and styled with Tailwind CSS v4.
- **Database**: MongoDB with Mongoose for robust data modeling.
- **File Uploads**: Support for uploading images/files via Multer.
- **API Testing**: Pre-configured Postman collection included.

## 🛠️ Tech Stack

### Client (`/quiz-client`)
- **Framework**: [Next.js 15](https://nextjs.org/)
- **Library**: [React 19](https://react.dev/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/)
- **Icons**: Lucide React
- **HTTP Client**: Axios
- **Real-time**: Socket.IO Client

### Server (`/server`)
- **Runtime**: Node.js
- **Framework**: [Express.js 5](https://expressjs.com/)
- **Database**: [MongoDB](https://www.mongodb.com/) (Mongoose)
- **Real-time**: Socket.IO
- **Authentication**: JSON Web Tokens (JWT) & bcrypt
- **File Handling**: Multer

## 📦 Project Structure

```text
Quizz/
├── quiz-client/                           # Next.js frontend application
├── server/                                # Node.js/Express backend server
└── quiz-server.postman_collection.json    # Postman collection for testing APIs
```

## ⚙️ Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB (Local instance or MongoDB Atlas)

### 1. Backend Setup

1. Navigate to the server directory:
   ```bash
   cd server
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file in the `server` directory and add your environment variables:
   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   ```
4. Start the development server:
   ```bash
   npm run dev
   ```
   *The server will typically start on `http://localhost:5000`.*

### 2. Frontend Setup

1. Navigate to the client directory:
   ```bash
   cd quiz-client
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the Next.js development server:
   ```bash
   npm run dev
   ```
   *The client application will typically start on `http://localhost:3000`.*

## 📄 API Documentation

A Postman collection is included in the root directory: `quiz-server.postman_collection.json`. 
You can import this file into [Postman](https://www.postman.com/) to easily explore and test the available REST API endpoints for the server.
