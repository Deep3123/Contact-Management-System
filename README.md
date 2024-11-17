# MERN Contact Management System

A **Contact Management System** built using the **MERN Stack**: MongoDB, Express.js, React.js, and Node.js.

---

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Application Structure](#application-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
    - [Backend Setup](#backend-setup)
    - [Frontend Setup](#frontend-setup)
- [Available Routes](#available-routes)
  - [Backend Routes](#backend-routes)
  - [Frontend Routes](#frontend-routes)
- [Contributing](#contributing)
- [License](#license)

---

## Overview
This application allows users to manage their contacts, offering features like creating, updating, deleting, and searching contacts. Secure user authentication ensures that each user’s data is protected.

---

## Features
- **User Authentication**: Secure sign-up and login with JWT-based authentication.
- **Contact CRUD**: Create, read, update, and delete contacts.
- **Search and Filter**: Quickly search and organize contacts.
- **Responsive Design**: Optimized for both desktop and mobile devices.

---

## Technologies Used
- **MongoDB**: NoSQL database for storing contacts and user data.
- **Express.js**: Backend web framework for API development.
- **React.js**: Frontend library for building the user interface.
- **Node.js**: JavaScript runtime for backend development.
- **JWT (JSON Web Tokens)**: Authentication and session management.
- **Bcrypt.js**: Password encryption for secure user credentials.

---

## Application Structure
The project is divided into two main parts:
1. **Frontend**: React.js application for managing contacts.
2. **Backend**: Express.js application for APIs, authentication, and database interaction.

---

## Getting Started

### Prerequisites
Ensure you have the following installed:
- [Node.js](https://nodejs.org/) - JavaScript runtime.
- [MongoDB](https://www.mongodb.com/) - NoSQL database (use a local instance or MongoDB Atlas).
- [npm](https://www.npmjs.com/) or [Yarn](https://yarnpkg.com/) - For managing dependencies.

---

### Installation

#### Backend Setup
1. Navigate to the `backend` directory:
   ```bash
   cd backend

2. Install dependencies:
   ```bash
   npm install

3. Create a `.env` file in the `backend` directory with the following variables:
   ```bash
   MONGODB_URI=<your_mongodb_connection_url>
   JWT_SECRET=<your_jwt_secret_key>

4. Start the backend server:
   ```bash
   npm start
   
The backend will run on `http://localhost:5000`.

#### Frontend Setup
1. Navigate to the `frontend` directory:
   ```bash
   cd frontend

2. Install dependencies:
   ```bash
   npm install

3. Start the React development server:
   ```bash
   npm start
   
The frontend will run on `http://localhost:3000`.

## Available Routes

### Backend Routes

#### User Authentication
- `POST /api/users/register` - Register a new user.
- `POST /api/users/login` - Login and receive a JWT token.

#### Contacts Management
- `GET /api/contacts` - Fetch all contacts for the authenticated user.
- `POST /api/contacts` - Create a new contact.
- `PUT /api/contacts/:id` - Update an existing contact.
- `DELETE /api/contacts/:id` - Delete a contact.

---

### Frontend Routes
- `/` - Home page (displays contacts).
- `/add` - Add a new contact.
- `/edit/:id` - Edit a contact.
- `/login` - Login page.
- `/register` - Registration page.
