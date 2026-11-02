# Intro to Backend Development - freeCodeCamp Tutorial

### Student Submission Details
* **Name:** Hardik Madhan
* **Enrollment No:** 250384
* **Course:** B.Tech
* **Section:** CSE-IV
* **Email:** hardik.madhan.25cse@bmu.edu.in

Hi there! This repository contains my implementation of the "Intro to Backend Development" video tutorial from the freeCodeCamp YouTube channel.

Tutorial Video: https://www.youtube.com/watch?v=KOutPbKc9UM  
Course Notes: https://excalidraw.com/#json=MZ-nK2h_8IKWFL0Nm1gxH,QJrqIq4vpqwtzvjh4YMFIA

## What was built in this project

* Understood what a backend is and its core components (Node runtime, Express framework, MongoDB database).
* Set up a Node.js project using ES Modules (`import`/`export`).
* Connected the Express application to MongoDB Atlas using Mongoose.
* Created database schemas and models for Users and Posts.
* Built user authentication (Register, Login, Logout) with password hashing using bcrypt.
* Implemented full CRUD operations (Create, Read, Update, Delete) for posts.
* Tested all endpoints using the Postman desktop app.

## How to run this project

### 1. Install dependencies:
```sh
npm install
```

### 2. Set up environment variables:
Create a `.env` file in the root folder (see `.env.example`):
```env
PORT=4000
MONGODB_URI="your_mongodb_connection_string_here"
```

### 3. Start the server:
Run in development mode (with nodemon):
```sh
npm run dev
```

The server will start on `http://localhost:4000`.

## API Endpoints

### Users (`/api/v1/users`)
* `POST /api/v1/users/register` - Register a user (hashes password with bcrypt)
* `POST /api/v1/users/login` - User login
* `POST /api/v1/users/logout` - User logout

### Posts (`/api/v1/posts`)
* `POST /api/v1/posts/create` - Create a new post
* `GET /api/v1/posts/getPosts` - Get all posts
* `PATCH /api/v1/posts/update/:id` - Update a post by ID
* `DELETE /api/v1/posts/delete/:id` - Delete a post by ID
