# ChatApp

ChatApp is a full-stack real-time chat application that allows users to communicate instantly. The project is built with a modern tech stack: **React + Vite** for the frontend, **Node.js/Express** for the backend API, **MongoDB** for data storage, and **Socket.io** for real-time messaging.

---

## Features

- **User Authentication:** Signup and login with hashed passwords.
- **Real-Time Messaging:** Send and receive messages instantly using Socket.io.
- **Online Presence:** See which users are online.
- **Responsive UI:** Built with Tailwind CSS and DaisyUI for modern, mobile-friendly design.
- **User Search:** Easily find users and start new chats.
- **Persistent Sessions:** JWT tokens stored in cookies.
- **Notifications:** Toast notifications for important actions (signup, login, logout, etc).

---

## Tech Stack

- **Frontend:** React, Vite, React Router, Axios, Tailwind CSS, DaisyUI, React Hook Form
- **Backend:** Node.js, Express.js, MongoDB (Mongoose), Socket.io, dotenv, cookie-parser, CORS
- **Authentication:** JWT (JSON Web Token)
- **Real-Time Engine:** Socket.io

---

## Getting Started

### Prerequisites

- Node.js & npm
- MongoDB instance (local or remote)

### Backend Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Shubhamrautela838/ChatApp.git
   cd ChatApp/Backend
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Create a `.env` file:**
   ```
   MONGODB_URI=your_mongodb_connection_string
   PORT=4001
   NODE_ENV=development
   JWT_SECRET=your_jwt_secret
   ```

4. **Run the backend server:**
   ```bash
   npm start
   ```
   The server runs on `http://localhost:4001`.

### Frontend Setup

1. **Go to the frontend folder:**
   ```bash
   cd Frontend
   ```

2. **Install frontend dependencies:**
   ```bash
   npm install
   ```

3. **Run the frontend in development:**
   ```bash
   npm run dev
   ```
   The app will be available at `http://localhost:3001`.

> In production, the frontend static build is served by the backend server.

---

## Folder Structure

```
ChatApp/
├── Backend/
│   ├── controller/
│   ├── models/
│   ├── routes/
│   ├── jwt/
│   ├── SocketIO/
│   ├── index.js
│   └── Frontend/
│       ├── src/
│       ├── index.html
│       ├── tailwind.config.js
│       └── vite.config.js
├── README.md
└── ...
```

---

## Usage

1. **Register:** Create a new account with your name, email, and password.
2. **Login:** Secure authentication with JWT.
3. **Chat:** See online users, select a user, and start chatting in real time.
4. **Logout:** End your session with one click.

---

## Deployment

- In `production`, set `NODE_ENV=production` in your `.env`.
- Build the frontend:
  ```bash
  cd Frontend
  npm run build
  ```
- The backend will serve the static frontend from `Frontend/dist`.

---

## License

[MIT](LICENSE) (add or change as appropriate)

---

## Maintainer

[Shubhamrautela838](https://github.com/Shubhamrautela838)

---

> _Update environment variables, license, and contact details as needed for your deployment._
