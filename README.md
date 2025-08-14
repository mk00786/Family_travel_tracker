# Family Travel Tracker

A **PostgreSQL-powered** mini-app built with **Node.js**, **Express**, and **EJS**, designed to help families visually track the countries they've visited.

---

## ​ Features

- Add visited countries with a simple form interface  
- View your travel log on a dynamic **EJS-rendered** page  
- Organized with modular directories like `public/` and `views/`  
- Clean and expressive UI for straightforward navigation

---

##  Technologies Used
-----------------------------------------------------
| Layer            | Stack                          |
|------------------|--------------------------------|
| Backend          | Node.js, Express               |
| Templating       | EJS                            |
| Database         | PostgreSQL                     |
| Development Tool | `dotenv` for environment config|
-----------------------------------------------------

---

##  Project Structure

family_travel_tracker/

├── public/ # Static assets (CSS, JS, images)

│ └── styles/ # Stylesheets

├── views/ # EJS view templates

├── .gitignore

├── index.js # Server entry point

├── package.json

└── package-lock.json

---

##  Prerequisites

Make sure you have installed:

- Node.js (v14 or above) and npm  
- PostgreSQL for data storage  
- Optionally, PgAdmin or similar tools for database management

---

##  Quick Setup Guide

1. **Clone the repository**
   ```bash
   git clone https://github.com/mk00786/Family_travel_tracker.git
   cd Family_travel_tracker

2. **Install Dependencies**
    npm install

3.  **Configure environment**
    Create a .env file at the project root:
    PG_USER=your_pg_user
    PG_PASSWORD=your_pg_password
    PG_HOST=localhost
    PG_PORT=5432
    PG_DATABASE=family_travel_db

4.  **Initialize the database**

Run psql or PgAdmin, then:

CREATE TABLE visits (
  id SERIAL PRIMARY KEY,
  country VARCHAR(255) NOT NULL,
  visited_at TIMESTAMP DEFAULT NOW()
);

5.  **Start the application**
npm start

6.  **Access in browser**
Visit http://localhost:3000 to add and view family travel logs


## Usage Tips

•	Add a country via the main form
•	View the updated country log list right away
•	UI should reflect visits in chronological order
## Optional Enhancements

•	Add user authentication for personalized travel logs
•	Create visual maps or charts to represent visited countries
•	Enable edit/delete for added entries
•	Deploy on platforms like Render or Heroku
