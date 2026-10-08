# 🌿 DestillApp — Backend

The backend API for **DestillApp**, a full-stack application for managing plant distillation processes and results.

Built with **Node.js, Express, GraphQL (Apollo Server), and MongoDB**, it provides API operations for plants, distillations, results, user accounts, and settings.

[← Back to the main README](../README.md)

---

## 🚀 Live API

**[GraphQL API — Render](https://destillapp.onrender.com/graphql)**

The backend is deployed on **Render**.

---

## 📌 API Overview

The GraphQL API supports operations involving:

- **Plants** — creating, retrieving, updating, and deleting plant records
- **Distillations** — managing distillation processes
- **Results** — storing and retrieving distillation results
- **Users** — authentication and profile management

### Example GraphQL Query

```graphql
query GetPlants {
  getPlants {
    _id
    plantName
    plantPart
    availableWeight
  }
}
```

---

## ✨ Features

### Authentication & Data Protection

- JWT-based user authentication
- User-specific data access
- Input validation and sanitization
- Centralized GraphQL error handling

### Data Management

- GraphQL queries and mutations for application data
- MongoDB persistence through Mongoose models
- Resolvers and schemas organized into separate modules

---

## 🛠️ Tech Stack

- **Node.js** — JavaScript runtime
- **Express** — HTTP server
- **GraphQL & Apollo Server** — API layer
- **MongoDB** — database
- **Mongoose** — data modeling
- **JWT** — authentication
- **validator** — input validation and sanitization
- **JSDoc** — API documentation

---

## 🏗️ Directory Structure

```text
backend/
├── src/
│   ├── app.js                    # Express server setup
│   ├── database/                 # Mongoose models
│   ├── graphql/
│   │   ├── resolvers/           # GraphQL resolvers
│   │   └── schemas/             # GraphQL type definitions
│   └── util/                    # Utility functions
│       ├── sanitization/        # Input sanitization
│       ├── authChecking.js      # Authentication middleware
│       ├── dataformating.js     # Data formatting utilities
│       └── dateformater.js      # Date formatting utilities
├── docs/                        # JSDoc documentation
├── triggers/                    # Database triggers
└── package.json
```

---

## ⚙️ Project Setup

### Install Dependencies

```sh
npm install
```

### Run the Server

```sh
npm start
```

---

## 🔧 Environment Variables

Create a `.env` file in the backend directory:

```env
# Database (MongoDB Atlas)
MONGODB_URI=mongodb+srv://your_username:your_password@cluster.mongodb.net/your_database

# JWT
JWT_SECRET=your_jwt_secret_key_here

# Server
PORT=3000

# CORS
ALLOWED_ORIGINS=http://localhost:5173,http://localhost:4173
```

Replace the placeholder values with your own configuration. Do not commit real credentials or secrets to the repository.

---

## 📚 Documentation

The backend uses **JSDoc** to generate documentation from the source code.

**[View Backend Documentation](https://destillapp.github.io/destill-app-fullstack/backend/)**

### Generate Documentation Locally

```sh
npm run docs:js
```

### View Documentation Locally

**Option 1: Open the generated HTML file**

Open `docs/jsdoc/index.html` in your browser.

**Option 2: Serve the documentation locally**

Install `serve` globally (one time only):

```sh
npm install -g serve
```

Serve the generated documentation:

```sh
npx serve docs/jsdoc
```

Then open the local URL displayed in the terminal (typically `http://localhost:3000`).

---

## 🔒 Security Features

- **Input sanitization** — uses the `validator` library to sanitize user input
- **JWT authentication** — token-based access to protected operations
- **GraphQL error handling** — centralized handling of application errors
- **User data isolation** — user-specific data access restrictions
