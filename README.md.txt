# MERN Task Tracker

A simple full-stack task management application built with the MERN stack (MongoDB, Express.js, React.js, and Node.js).

---

## Project Description

**MERN Task Tracker** is a web application that helps users organize their daily work. Users can create tasks, view them in a list, mark them as completed, edit them, and delete them when they are no longer needed.

The project is split into two parts:

- **Frontend (Client):** A React.js app that users interact with in the browser.
- **Backend (Server):** A Node.js and Express.js REST API that handles requests and talks to the database.
- **Database:** MongoDB stores all task data.

---

## Project Purpose

The purpose of this project is to:

- Practice building a complete full-stack application from start to finish.
- Understand how the frontend, backend, and database communicate with each other.
- Learn the basics of CRUD operations (Create, Read, Update, Delete).
- Gain hands-on experience with Git and GitHub for version control and project documentation.
- Build a beginner-friendly project that can be extended with more features over time.

---

## Frontend Development Plan

The frontend will be built with **React.js**.

### Planned Pages and Components

- **App Component:** The main component that holds the whole application.
- **Header:** Displays the application title.
- **Task Form:** A form to add a new task (title and optional description).
- **Task List:** Displays all tasks fetched from the backend.
- **Task Item:** Shows a single task with buttons to complete, edit, or delete it.

### Planned Features

- Add a new task using a form.
- Display all tasks in a clean list.
- Mark a task as completed or pending.
- Edit an existing task.
- Delete a task.
- Show simple messages for loading and errors.

### Development Steps

1. Create the React app (using Vite or Create React App).
2. Set up the folder structure for components.
3. Build the Task Form, Task List, and Task Item components.
4. Use `useState` and `useEffect` to manage data and fetch tasks.
5. Connect the frontend to the backend API using `fetch` or `axios`.
6. Add basic CSS styling to make the app clean and easy to use.

---

## Backend Development Plan

The backend will be built with **Node.js** and **Express.js**.

### Planned API Endpoints

| Method | Endpoint         | Description            |
|--------|------------------|------------------------|
| GET    | `/api/tasks`     | Get all tasks          |
| GET    | `/api/tasks/:id` | Get a single task      |
| POST   | `/api/tasks`     | Create a new task      |
| PUT    | `/api/tasks/:id` | Update an existing task|
| DELETE | `/api/tasks/:id` | Delete a task          |

### Development Steps

1. Initialize the Node.js project with `npm init`.
2. Install required packages: `express`, `mongoose`, `cors`, `dotenv`, and `nodemon`.
3. Create the Express server and set up middleware.
4. Connect the server to MongoDB using Mongoose.
5. Create the Task model, routes, and controllers.
6. Add basic error handling and input validation.
7. Test all endpoints using Postman or Thunder Client.

### Suggested Folder Structure

```
mern-task-tracker/
├── client/          # React frontend
│   └── src/
│       ├── components/
│       └── App.js
├── server/          # Node/Express backend
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   └── server.js
└── README.md
```

---

## Database Plan

The project will use **MongoDB** to store data, with **Mongoose** to define the structure of the data.

### Task Schema

| Field         | Type    | Description                          |
|---------------|---------|--------------------------------------|
| `title`       | String  | The name of the task (required)      |
| `description` | String  | Extra details about the task         |
| `completed`   | Boolean | Whether the task is done (default: `false`) |
| `createdAt`   | Date    | Automatically added when created     |
| `updatedAt`   | Date    | Automatically updated when edited    |

### Database Notes

- MongoDB Atlas (cloud) or a local MongoDB installation can be used.
- The database connection string will be stored in a `.env` file and **never** uploaded to GitHub.
- Mongoose timestamps will be used to track creation and update times.

---

## Technologies Used

- **MongoDB** – NoSQL database for storing tasks
- **Express.js** – Web framework for building the backend API
- **React.js** – JavaScript library for building the user interface
- **Node.js** – JavaScript runtime for running the server
- **Mongoose** – Library for modeling MongoDB data
- **Axios / Fetch API** – For sending requests from the frontend to the backend
- **Git & GitHub** – Version control and project hosting
- **Postman / Thunder Client** – For testing API endpoints
- **VS Code** – Code editor

---

## Future Improvements

- Add user registration and login (authentication with JWT).
- Allow each user to see only their own tasks.
- Add task due dates and priority levels (Low, Medium, High).
- Add task categories or labels.
- Add search and filter options (by status, date, or priority).
- Add drag-and-drop to reorder tasks.
- Improve the design and make it fully mobile responsive.
- Add a dark mode option.
- Write unit tests for the frontend and backend.
- Deploy the app online (for example, Render, Vercel, or Netlify).

---

## Project Goal

The main goal of **MERN Task Tracker** is to build a working, easy-to-understand full-stack application that demonstrates the core concepts of the MERN stack. By completing this project, I aim to strengthen my understanding of web development, REST APIs, databases, and GitHub workflows, and to create a solid foundation for building larger and more advanced projects in the future.

---

## Author

**Your Name**
GitHub: [your-username](https://github.com/your-username)