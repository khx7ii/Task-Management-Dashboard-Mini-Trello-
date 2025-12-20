# 🗂️ Task Management Dashboard (Mini Trello)

## 📌 Project Overview
This project is a **Task Management Dashboard** inspired by Trello and Asana (simplified version).  
It is a **Single Page Application (SPA)** built using **React**, where users can view projects and manage tasks across different statuses.

Projects and initial tasks are fetched from a **free public API**, while adding, deleting, and updating tasks/projects are handled locally using React state.

---

## 🚀 Main Features

### 1️⃣ Dashboard – Projects List Page (`/`)
- Display a list of projects fetched from an API.
- Each project is shown using a **ProjectCard** component.
- Project card includes:
  - Project title
  - Short description
  - Number of tasks
  - **View Tasks** button
- Button to navigate to **Add Project** page.

---

### 2️⃣ Project Tasks Page (`/project/:id`)
- Display the selected project title.
- Show tasks organized into three columns:
  - **To Do**
  - **In Progress**
  - **Done**
- Each task is displayed using a **TaskCard** component containing:
  - Title
  - Description
  - Status
  - Actions
- Features:
  - Move tasks between columns (local state).
  - Delete tasks.
- Button to navigate to **Add Task** page.

---

### 3️⃣ Add Task Page (`/add-task`)
- Form fields:
  - Task Title
  - Task Description
  - Select Project (dropdown)
  - Select Status (To Do / In Progress / Done)
- On submit:
  - Task is added to local state.
  - User is redirected to the selected project page.

---

### 4️⃣ Add Project Page (`/add-project`)
- Form fields:
  - Project Title
  - Project Description
- On submit:
  - Project is added to local state.
  - User is redirected to the Dashboard.

---

## 🌐 API Requirements
- handled API using MockAPI
- API returns data in JSON format.
- Only **GET requests** are used.
- Adding, deleting, and editing are handled locally in React.

## 🧠 State Management
- React `useState` and `useEffect` are used.
- Tasks and projects are managed locally after fetching.
- State updates dynamically when tasks are added, moved, or deleted.

---

## 👥 Team Structure
- **[Omnia Alwan](https://github.com/Omnia-Alwan):** Routing & Layout (Navbar, page structure)
- **[Kholod Elhmamsy](https://github.com/khx7ii):** UI Components (ProjectCard, TaskCard, Columns)
- **[Heba Salhien](https://github.com/hebasalhien):** API & State Logic (fetching and organizing data)
- **[Amira Mohamed](https://github.com/AmiraMohamedM):** Forms (Add Task, Add Project)

---

## 🛠️ Technologies Used
- React
- React Router DOM
- JavaScript (ES6)
- HTML5
- CSS / Bootstrap / Tailwind

> ❌ UI libraries like Material UI or Ant Design are **not used**.

---

## ⭐ Bonus Features
- 🔍 Search for tasks
- 🌙 Dark mode
- 🖱️ Drag & Drop tasks
- 💾 Save data to LocalStorage

---

## ▶️ How to Run the Project

1. Clone the repository:
```bash
git clone https://github.com/5l5ola/Task-Management-Dashboard-Mini-Trello-.git
