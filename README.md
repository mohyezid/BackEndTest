# Task Management Application API

Objective: Build a complex RESTful API using Javascript, Express.js, JWT authentication, PostgreSQL, and Prisma ORM for a sophisticated task management application. the time given to complete this exam is maximum of 7 days.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Testing](#testing)
- [API Documentation](#api-documentation)
- [License](#license)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Node.js and npm installed
- Database (e.g., PostgreSQL) installed and running

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/MYzbest/BackEndTest.git
   ```

2. Change into the project directory:

   ```bash
   cd Task-Management-App
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Set up the environment variables:

   ```bash
   # Create a copy of the sample environment file
   cp .env.example .env

   # Edit the .env file and provide necessary configurations
   ```

   Ensure to fill in the required environment variables such as `DATABASE_URL`, `JWT_SECRET`, etc.

5. Run database migrations:

   ```bash
   npx prisma migrate dev
   ```

## Usage

Run the server with the following command:

```bash
npm start
```

## Testing

Run the tests with the following command:

```bash
npm test
```

## API Documentation

[Link to Postman Documentation](https://documenter.getpostman.com/view/22088588/2s9YsFFEQQ)

## Built With

- Node.js
- Express
- Prisma
- PostgreSQL

## Features

- User Authentication
- Authentication Middleware
- Implementing role-based access control with user and admin roles
- Implementing an endpoint to retrieve the user's profile information, including projects and tasks.
- Task Assignments
- File Uploads
- Real-time Updates
- Search and Filter

## API Endpoints

### User Endpoints

- POST /api/auth: Register a new user
- POST /api/auth/login: Log in a user

### Task Endpoints

- GET /api/tasks/:taskId: Fetch a specific task by ID
- PUT /api/tasks/:taskId: Update a specific task by ID
- DELETE /api/tasks/:taskId: Delete a specific task by ID

### Project Endpoints

- GET /api/projects: Fetch all projects for the authenticated user
- GET /api/projects/:projectId: Fetch a specific project by ID
- POST /api/projects/:projectId/tasks: Create a new task within a project
- DELETE /api/projects/:projectId: Delete a specific project by ID

## License

This project is licensed under the [Mohammed](LICENSE.md) - see the [LICENSE.md](LICENSE.md) file for details.
