# Fitness Coaching and Tracking App

A Vue 3 + Firebase web application for fitness coaching, routine and diet assignment, progress tracking, appointments, and role-based access.

This project includes authentication, protected routes, user and admin workflows, progress visualization, and Firebase integration for data and file management. It is designed as a fitness management platform where users can follow assigned plans and track their progress, while admins can manage routines, diets, and appointments.

> **Current scope**: authentication, role-based access, user and admin views, routine and diet assignment, progress tracking, appointment management, charts, and Firebase-based persistence.

---

## Contents

- [Key Features](#key-features)
- [Architecture and Stack](#architecture-and-stack)
- [Project Structure](#project-structure)
- [Core Modules](#core-modules)
- [Requirements](#requirements)
- [Environment Variables](#environment-variables)
- [Quick Start](#quick-start)
- [Running the App](#running-the-app)
- [Main Views](#main-views)
- [Notes](#notes)
- [Screenshots](#screenshots)

---

## Key Features

- User authentication with Firebase Auth
- Role-based access for users and admins
- Protected routes with Vue Router
- Global state management with Pinia
- Routine assignment and tracking
- Diet assignment and management
- Progress tracking with charts and visual summaries
- Appointment scheduling and management
- File and media handling with Firebase Storage
- Cloud persistence with Firestore

---

## Architecture and Stack

- **Frontend**: Vue 3
- **Routing**: Vue Router
- **State Management**: Pinia
- **Backend Services**: Firebase
- **Authentication**: Firebase Authentication
- **Database**: Cloud Firestore
- **Storage**: Firebase Storage
- **Build Tool**: Vite
- **Package Manager**: pnpm

---

## Project Structure

```text
/src
  /assets        Static assets
  /components    Reusable UI components
  /router        Route definitions and navigation guards
  /stores        Pinia stores
  /views         Main application views
  /firebase      Firebase configuration and setup
/public          Public static files
```

> The exact structure may vary slightly depending on the current branch or local version of the project.

---

## Core Modules

### Authentication
Handles login, session persistence, and access control through Firebase Authentication.

### User Area
Provides the user-facing flows to review assigned routines, diets, appointments, and progress.

### Admin Area
Provides admin-oriented views and workflows for assigning plans, managing users, and organizing fitness-related records.

### Progress Tracking
Displays progress information through charts and visual summaries.

### Storage and Persistence
Uses Firestore for structured data and Firebase Storage for file handling where applicable.

---

## Requirements

- Node.js 18+
- pnpm
- Firebase project credentials

---

## Environment Variables

Create a `.env` file based on your Firebase project configuration.

```env
VITE_FIREBASE_API_KEY=your_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
```

> Use your own Firebase project values. Do not commit real secrets or production configuration unnecessarily.

---

## Quick Start

This project uses [pnpm](https://pnpm.io/).

```bash
git clone <your-repository-url>
cd Fitness-main
pnpm install
pnpm run dev
```

---

## Running the App

Start the development server:

```bash
pnpm run dev
```

The app will usually be available at:

```text
http://localhost:5173
```

To create a production build:

```bash
pnpm run build
```

To preview the production build locally:

```bash
pnpm run preview
```

---

## Main Views

Depending on the current implementation, the application includes views such as:

- login / authentication
- user dashboard
- admin dashboard
- routines
- diets
- appointments
- progress tracking
- profile-related sections

These flows are protected according to the authenticated user role.

---

## Notes

- The project uses Firebase as the main backend service layer.
- Route access depends on authentication state and user role.
- Firestore is used for application data persistence.
- Firebase Storage is used for file-related features where applicable.
- Environment variables should be used for Firebase configuration instead of hardcoding values directly in the source code.

---

## Screenshots

![App Screenshot](./preview.png)
