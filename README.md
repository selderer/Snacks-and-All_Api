# 🍩 Snacks and All: API

The small **Node.js server** behind the online snack shop **Snacks and All**. It stores the products, handles product image uploads and protects the admin area with a login.

> 🖥️ **This is the server part.** The website itself is in the client repo: **[Snacks-and-All-Client](https://github.com/selderer/Snacks-and-All-Client)** ([live demo](https://selderer.github.io/Snacks-and-All-Client/)).

Built as part of my college diploma project (2024). It's a small API, and it was my first hands-on practice with Node.js, Express and a SQL database.

---

## 🔧 What it does

- 📦 Serves the **product data** shown on the shop website
- 🖼️ Accepts **product image uploads** from the admin page
- 🔐 **Admin login**: passwords are stored hashed, and logged-in sessions use secure tokens

---

## 🧰 Tech stack

| Tool | Used for |
|---|---|
| **Node.js + Express** | The web server and API |
| **MySQL** | The database |
| **JWT** (`jsonwebtoken`) | Admin login tokens |
| **bcrypt** | Password hashing |
| **Multer** | Image uploads |
| **CORS** | Letting the website talk to the API |

---

## 🏗️ How it fits together

```
 React website (Snacks-and-All-Client)  ──►  This API  ──►  MySQL database
```

## 📁 Project structure

```
controllers/   → the logic behind each request
routes/        → the API endpoints
connect.js     → database connection
index.js       → server entry point
```

---

## 🚀 Run it locally

You need **Node.js 20.6 or newer** and a running **MySQL** database.

```bash
git clone https://github.com/selderer/Snacks-and-All_Api.git
cd Snacks-and-All_Api
npm install
```

Create a `.env` file in the project root. Use `.env.development` as a template for the variable names, and fill in your own database details and secrets.

```bash
npm start
```

Then run the [client](https://github.com/selderer/Snacks-and-All-Client) so the website can use the API.

---

## 👤 Author

**selderer**: [GitHub profile](https://github.com/selderer)
