# QueueLess - Hospital OPD Queue Management System

A comprehensive web application for managing hospital OPD queues, reducing waiting times, and providing real-time updates to patients, doctors, and staff.

## 🚀 Getting Started

Follow these instructions to set up the project locally.

### Prerequisites

- **Node.js** (v14 or higher)
- **MongoDB** (Local or Atlas URI)
- **Git**

### 1. Installation

Clone the repository or extract the zip file:

```bash
git clone https://github.com/Harsh-sh7/QueueLess.git
cd QueueLess
```

### 2. Backend Setup

Navigate to the backend directory and install dependencies:

```bash
cd backend
npm install
```

**Create Environment File:**
Create a `.env` file in the `backend` directory with the following variables:

```env
PORT=5001
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
CLIENT_URL=http://localhost:5173
```
*Note: Replace `your_mongodb_connection_string` with your actual MongoDB URI.*

Start the backend server:

```bash
npm start
# or for development with auto-reload:
npm run dev
```

### 3. Frontend Setup

Open a new terminal, navigate to the frontend directory, and install dependencies:

```bash
cd frontend
npm install
```

**Create Environment File:**
Create a `.env` file in the `frontend` directory:

```env
VITE_API_URL=http://localhost:5001/api
```

Start the frontend development server:

```bash
npm run dev
```

### 4. Running the Application

- **Backend**: Runs on http://localhost:5001
- **Frontend**: Runs on http://localhost:5173 (or similar port allocated by Vite)

Open the frontend URL in your browser to access the application.

## 📂 Project Structure

- `backend/`: Node.js + Express server, MongoDB models, API routes.
- `frontend/`: React + Vite application, UI components, pages.

## 🔑 Default Roles (for testing)

You may need to seed the database or register new users.
- **Admin**: Has access to doctor management and analytics.
- **Doctor**: Manages their specific queue and session.
- **Staff**: Manages emergency status and specific queues.
- **Patient**: Joins queues and views status.

## 🛠 Tech Stack

- **Frontend**: React, Vite, TailwindCSS, Lucide Icons, React Query.
- **Backend**: Node.js, Express, MongoDB, Mongoose, Socket.io, JWT.
