# 🌍 Capitals Quiz Game

A full-stack web quiz application built with **Node.js**, **Express**, and **PostgreSQL** where users identify the **capital city** of a given country. The app demonstrates database integration using the `pg` module and serves as a learning project for connecting a Node.js backend with a PostgreSQL database.

---

## 📸 Demo
![Screenshot 2025-06-16 200929](https://github.com/user-attachments/assets/2d0cffe9-cd56-44cd-881c-cef499d188b5)

![image](https://github.com/user-attachments/assets/ce75da41-c80f-45cb-a1e8-75f6f1806634)
--

## ✨ Features

- Displays a country and prompts the user to enter its capital city.
- Score is incremented for each correct answer.
- The game ends on a wrong answer, and the final score is shown.
- Flags or country names are pulled from a **PostgreSQL database**.
- Clean and responsive UI using HTML and CSS.
- Middleware usage for static files and form parsing.

---

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/capitals-quiz.git
cd capitals-quiz

# Install dependencies
npm install




🧠 Database Setup
Ensure PostgreSQL is installed and running on your machine.

1. Create a database named world:

sql
CREATE DATABASE world;
Create a capitals table with the following structure:

sql
CREATE TABLE capitals (
  id SERIAL PRIMARY KEY,
  country VARCHAR(255) NOT NULL,
  capital VARCHAR(255) NOT NULL,
  flag TEXT -- optional, if you're displaying flag emojis or images
);


IMPORT the Capitals.csv file to the TABLE.

js

const db = new pg.Client({
  user: "postgres",
  host: "localhost",
  database: "world",
  password: "your_password",
  port: 5432 // or your PostgreSQL port
});

PROJECT STRUCTURE:

capitals-quiz/
│
├── public/
│   └── styles/
│       └── main.css
│
├── views/
│   └── index.ejs
│
├── index.js
├── package.json
└── README.md

🧰 Technologies Used

Node.js, Express.js, PostgreSQL, pg(node-postgres), EJS, HTML5 & CSS3


💡 Learning Outcomes
This project is a great demonstration of:

Connecting a PostgreSQL database to a Node.js application.

Using Express routing and middleware.

Managing form submissions and HTTP requests.

Rendering dynamic HTML using EJS templating.

Structuring full-stack applications.

