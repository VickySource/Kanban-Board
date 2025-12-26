🗂️ Kanban Board Application (MERN Stack)

A full-stack Kanban Board application built with React, Node.js, Express, and MongoDB.
It helps teams manage tasks visually across multiple sections with authentication, drag & drop support, and a responsive UI.

🚀 Overview

This project provides a complete Kanban workflow where users can:

Sign up and log in securely

Create and manage sections and tasks

Move tasks between sections using drag & drop

Collaborate with multiple users

Both frontend and backend are included in this single repository.

📂 Project Structure
kanban-board/
├── frontend/        # React + Material UI frontend
├── backend/         # Node.js + Express backend
├── README.md
└── .gitignore

✨ Features
🔐 Authentication

User signup & login

JWT-based authentication

Persistent login sessions

User profile with avatar

Total member count display

🗂️ Section Management

Default sections:

📝 Todo

🛧 In Progress

✅ Done

Add custom sections

Update or delete sections

✅ Task Management

Create tasks with:

Task title

Description

Due date

Assignee

Update and delete tasks

View tasks by section

🔄 Drag & Drop

Move tasks between sections

Automatically updates task status

📱 Responsive Design

Desktop, tablet, and mobile support

Mobile drawer navigation

Clean Material UI layout

🛠️ Technologies Used
Frontend

React

Redux Toolkit

Material UI (MUI)

Axios

Backend

Node.js

Express.js

MongoDB

Mongoose

JWT Authentication

⚙️ Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/VickySource/Kanban-Board.git
cd kanban-board

2️⃣ Backend Setup
cd backend
npm install


Create a .env file inside backend/:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key


Start the backend server:

npm start


Backend runs on:

http://localhost:5000

3️⃣ Frontend Setup
cd ../frontend
npm install
npm run dev


Frontend runs on:

http://localhost:5173

🔌 API Endpoints
Authentication

POST /api/auth/signup – Register user

POST /api/auth/login – Login user

GET /api/auth/me – Get current user

GET /api/auth/count – Get total users

Sections

POST /api/section – Create section

GET /api/section – Get all sections

PUT /api/section/:id – Update section

DELETE /api/section/:id – Delete section

Tasks

POST /api/task – Create task

GET /api/task/:section – Get tasks by section

PUT /api/task/:id – Update task

DELETE /api/task/:id – Delete task

PATCH /api/task/move – Move task between sections

🔐 Environment Variables

Ensure .env files are not committed to GitHub.

Required:

PORT

MONGO_URI

JWT_SECRET

👥 Team Members

Vikas A R

Sufiyan

Tejaswini

Vasantha

📌 Future Enhancements

Role-based access control

Real-time updates (Socket.io)

Task comments and activity logs

Board sharing & permissions

Deployment (Vercel + Render)

⭐ Support

If you like this project, give it a ⭐ on GitHub — it helps more than debugging at 2 AM 😄
