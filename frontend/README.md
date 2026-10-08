# 🌿 DestillApp — Frontend

The frontend application for **DestillApp**, a full-stack web application for managing plant distillation processes and their results.

Built with **Vue 3, TypeScript, Vuex, Vuetify, Apollo Client, and Vite**, it provides the user interface for interacting with the application's GraphQL API.

[← Back to the main README](../README.md)

---

## 🚀 Live Demo

**[Try DestillApp](https://destillapp.netlify.app/)**

The frontend is deployed on **Netlify**.

---

## ✨ Features

The frontend provides an interface for:

- Working with plant-related data
- Managing distillation processes
- Viewing and managing distillation results
- User authentication and account management

The application communicates with the backend through **Apollo Client and GraphQL**.

---

## 🛠️ Tech Stack

- **Vue 3 + TypeScript** — frontend framework and type safety
- **Vuetify** — Material Design UI components
- **Vuex** — centralized state management
- **Apollo Client** — GraphQL integration
- **Vite** — development server and build tooling
- **Sentry** — error and performance monitoring
- **VitePress** — project documentation

---

## ⚙️ Project Setup

### Install Dependencies

```sh
npm install
```

### Run in Development Mode

```sh
npm run dev
```

### Build for Production

```sh
npm run build
```

### Lint and Fix Files

```sh
npm run lint
```

### Run Unit Tests

```sh
npx vitest run
```

---

## 📚 Documentation

**[View Frontend Documentation](https://destillapp.github.io/destill-app-fullstack/)**

The project uses VitePress for documentation, with additional tooling for generating TypeScript API and Vue component documentation.

### Build and Preview Documentation Locally

```sh
npm run docs:build
npm run docs:dev
```

### Generate TypeScript API Documentation

```sh
npx typedoc
```

### Generate Vue Component Documentation

```sh
npm run docs:vue
```

---

## 📦 Directory Structure

```text
frontend/
├── src/             # Source code (components, pages, store, etc.)
├── docs/            # VitePress documentation
├── public/          # Static assets
├── scripts/         # Utility scripts (e.g., doc generation)
├── package.json     # Project metadata and scripts
├── vite.config.ts   # Vite configuration
└── tsconfig.json    # TypeScript configuration
```

---

## 🔧 Environment Variables

Create a `.env` file in the frontend directory:

```env
VITE_GRAPHQL_URI=YOUR_GRAPHQL_ENDPOINT
VITE_SENTRY_DSN=YOUR_SENTRY_DSN
```

Replace the placeholders with the appropriate values for your environment.

---

## 🐞 Error Reporting

**Sentry** is integrated for error and performance monitoring.

Set `VITE_SENTRY_DSN` in your `.env` file to enable monitoring.
