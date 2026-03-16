# 📝 To-Do List App

A simple **full-stack To-Do List application** where users can add, edit, and delete tasks.
All tasks are stored in a PostgreSQL database and displayed dynamically using EJS templates.

---

# 🚀 Features

* Add new tasks
* Edit existing tasks
* Delete tasks
* Store tasks in PostgreSQL database
* Dynamic rendering with EJS
* Clean and simple UI

---

# 🛠 Tech Stack

* Node.js
* Express.js
* PostgreSQL
* EJS
* Body Parser

---

# 📂 Project Structure

```
To-Do-List-App
│
├── public/
│   └── assets/icons
│
├── views/
│   ├── partials/
│   │   ├── header.ejs
│   │   └── footer.ejs
│   │
│   └── index.ejs
│
├── index.js
├── package.json
└── README.md
```

---

# ⚙️ Prerequisites

Install the following software before running the project.

### 1️⃣ Install Node.js

https://nodejs.org/

### 2️⃣ Install PostgreSQL

https://www.postgresql.org/download/

---

# 🗄️ Database Setup

Open PostgreSQL and create a database.

```sql
CREATE DATABASE todo_app;
```

Create the required table:

```sql
CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title TEXT NOT NULL
);
```

---

# 🔑 Configure PostgreSQL Login

Open **index.js** and update your PostgreSQL credentials:

```javascript
const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "todo_app",
  password: "your_password",
  port: 5432,
});
```

Make sure the login credentials match your PostgreSQL installation.

---

# 📦 Installation

Clone the repository:

```
git clone https://github.com/yourusername/To-Do-List-App.git
cd To-Do-List-App
```

Install dependencies:

```
npm install
```

---

# ▶️ Run the Application

Start the server:

```
node index.js
```

Open your browser and go to:

```
http://localhost:3000
```

---

# 📸 How It Works

1. Enter a task in the input box.
2. Click **+** to add the task.
3. Click the **pencil icon** to edit the task.
4. Click the **checkbox** to delete the task.

---

# 🧠 What This Project Demonstrates

* Building a backend server with Express
* Connecting Node.js to PostgreSQL
* CRUD operations using SQL
* Server-side rendering using EJS
* Handling form requests

---
