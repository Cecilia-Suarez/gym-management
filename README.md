🥊Gym Management System🥊

Desktop application for managing gym members, built for real-world usage at **300 Academia de Boxeo**.

---

## 1- Overview

This project is a redesigned version of a previously used system at **300 Academia de Boxeo**, rebuilt with a modern and scalable architecture.

The goal is to replace legacy workflows with a maintainable, production-oriented solution.

### Core features

* Member registration and management
* Data editing and listing
* Membership expiration tracking

---

## 2- Architecture

The application follows a modular architecture with clear separation of concerns:

Desktop (Tauri - planned)
→ Frontend (React + TypeScript)
→ Backend (Go REST API)
→ Database (PostgreSQL)

The backend runs locally and exposes a REST API consumed by the frontend.

---

## 3- Tech Stack

### Frontend

* React (Vite)
* TypeScript
* Tailwind CSS
* TanStack Query (server state management)

### Backend

* Go (Golang)
* Gin (HTTP framework)
* sqlx (data access layer)

### Database

* PostgreSQL
* Migration-based schema management

### Infrastructure

* Docker & Docker Compose

### Tooling

* Prettier
* Husky + Commitlint
* Semantic Release

---

## 4- Project Structure

```
root/
├── frontend/     # React application
├── backend/      # Go API
├── database/     # Migrations & seeds
├── docker/       # Docker configuration
├── docs/         # Documentation
```

---

## 5- Development Workflow

### Branching strategy

* `main` → production-ready code
* `dev` → integration branch
* `feature/*` → feature development

Workflow:
feature → dev → main

---

## 6- Versioning & Releases

This project uses **Semantic Versioning** with automated releases.

* `feat` → minor version
* `fix` → patch version
* `BREAKING CHANGE` → major version

Automated with:

* semantic-release
* GitHub releases
* CHANGELOG generation

---

## 7- Code Quality

* Conventional Commits enforced
* Commit validation via Husky + Commitlint
* Consistent formatting with Prettier

---

## 8- Local Setup

### 1. Start database

```bash
docker-compose up -d
```

### 2. Run backend

```bash
cd backend
go run main.go
```

### 3. Run frontend

```bash
cd frontend
npm install
npm run dev
```

---

## 9- Roadmap

* Feature-based frontend architecture
* REST API design (handlers / services / repositories)
* Full system integration (frontend ↔ backend ↔ database)
* Desktop packaging with Tauri 

---

## 10- Engineering Focus

This project emphasizes:

* Scalable architecture
* Separation of concerns
* Maintainability over quick solutions
* Real-world development practices

---
