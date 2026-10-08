# 🌿 DestillApp — Essential Oil Distillation Manager

DestillApp is a full-stack web application for managing plant distillation processes, results, and user accounts.

The application combines a **Vue 3 and TypeScript frontend** with a **Node.js, Express, GraphQL, and MongoDB backend**.

It was developed to support the organization and tracking of plant distillation data through a dedicated web interface.

---

## 🚀 Live Demo

**[Try DestillApp](https://destillapp.netlify.app/)**

- **Frontend:** Deployed on Netlify
- **Backend:** Deployed on Render
- **Demo access:** Click **"Wypróbuj Demo"** in the application or use the credentials below.

```text
Email: demoUser@mail.com
Password: demoPassword123
```

---

## 📌 Project Overview

DestillApp provides an interface for working with:

- **Plants** — plant-related data used in distillation processes
- **Distillation processes** — information about individual distillations
- **Results** — data recorded from distillation processes
- **User accounts** — authentication and account management

The frontend communicates with the backend through a GraphQL API.

---

## 🛠️ Tech Stack

### Frontend

- Vue 3
- TypeScript
- Vite
- Vuetify
- Vuex
- Apollo Client

### Backend

- Node.js
- Express
- GraphQL
- Apollo Server
- MongoDB
- Mongoose
- JWT authentication

### Deployment

- Netlify — frontend
- Render — backend

---

## 🏗️ Project Structure

```text
frontend/    Vue 3 application
backend/     Node.js and GraphQL API
```

The project is organized into separate frontend and backend applications, each with its own README and technical documentation.

---

## 💻 Frontend

The frontend provides a type-safe user interface for managing distillation-related data.

It uses **Vue 3 and TypeScript**, **Vuetify** for UI components, **Vuex** for state management, and **Apollo Client** to communicate with the GraphQL API.

**Documentation:**

- [Frontend README](frontend/README.md)
- [Frontend VitePress Docs](https://destillapp.github.io/destill-app-fullstack/)

---

## ⚙️ Backend

The backend provides a GraphQL API for managing distillation processes, plants, results, users, and application settings.

It uses **Node.js**, **Express**, **Apollo Server**, and **MongoDB with Mongoose**.

The API includes JWT authentication, input validation and sanitization, and a modular structure for GraphQL schemas and resolvers.

**Documentation:**

- [Backend README](backend/README.md)
- [Backend JSDoc Docs](https://destillapp.github.io/destill-app-fullstack/backend/)

---

## 📚 Further Documentation

For setup instructions, implementation details, and additional technical information, see the dedicated frontend and backend documentation linked above.
