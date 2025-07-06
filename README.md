# 📝 To-Do List App with PostgreSQL & Express.js

This is a full-stack to-do list web application built with **Node.js**, **Express**, **PostgreSQL**, and **EJS**. Users can view, add, edit, and delete tasks — all stored persistently in a PostgreSQL database.

---

## 🚀 Features

- Add new tasks
- Edit existing tasks
- Delete tasks
- View all tasks sorted by ID
- Uses EJS for server-side rendering
- Connects to a PostgreSQL database

---

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: PostgreSQL
- **Templating**: EJS
- **Middleware**: Body-parser

---

## 📁 Project Structure

todo-app/
│
├── public/ # Static files (CSS, JS, images if any)
├── views/
│ └── index.ejs # Main UI template
├── app.js # Main Express application (your code)
├── package.json
└── README.md

---

## 🗃️ PostgreSQL Setup

Ensure you have a PostgreSQL database named `world` with a table called `items`.

```sql
CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title TEXT NOT NULL
);

📦 Installation
Clone the repository:
git clone https://github.com/your-username/todo-app.git
cd todo-app

Install dependencies:
npm install
Configure PostgreSQL connection inside app.js:

const db = new pg.Client({
  user: "your_pg_username",
  host: "localhost",
  database: "world",
  password: "your_pg_password",
  port: 5432,
});


Start the application:
node app.js
Open in browser:
http://localhost:3000
