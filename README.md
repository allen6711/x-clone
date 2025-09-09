# [Your Project Name Here]

 A full-stack social media application inspired by modern platforms like X (formerly Twitter). This project allows users to sign up, create posts, follow other users, and engage with content through likes and comments. It is built with a decoupled architecture, featuring a React frontend and a Node.js/Express backend.


---

## 🚀 Features

* **User Authentication**:
    * User registration and login functionality.
    * Secure, stateless authentication using JSON Web Tokens (JWT).
    * Protected routes accessible only to authenticated users.
* **User Profiles**:
    * View and edit user profiles, including username, bio, profile picture, and cover image.
    * Follow and unfollow other users.
    * View user-specific post feeds.
* **Post Management**:
    * Create and delete posts.
    * Like and unlike posts.
    * Comment on posts.
    * Browse various feeds: all posts, posts from followed users, and liked posts.
* **Notification System**:
    * Receive real-time notifications for likes, comments, and new followers.
    * View and clear notifications.

---

## 🛠️ Tech Stack

### **Backend**
* **[Node.js](https://nodejs.org/)**: JavaScript runtime environment
* **[Express.js](https://expressjs.com/)**: Web framework for building RESTful APIs
* **[MongoDB](https://www.mongodb.com/)**: NoSQL database for data storage
* **[Mongoose](https://mongoosejs.com/)**: Object Data Modeling (ODM) library for MongoDB
* **[JSON Web Token (JWT)](https://jwt.io/)**: For implementing user authentication
* **[bcryptjs](https://www.npmjs.com/package/bcryptjs)**: For password hashing
* **[Cloudinary](https://cloudinary.com/)**: For cloud-based image uploads and storage

### **Frontend**
* **[React](https://reactjs.org/)**: JavaScript library for building user interfaces
* **[Vite](https://vitejs.dev/)**: Next-generation frontend tooling for fast development
* **[Tailwind CSS](https://tailwindcss.com/)**: A utility-first CSS framework
* **[React Router](https://reactrouter.com/)**: For client-side routing
* **[TanStack Query (React Query)](https://tanstack.com/query/latest)**: For data fetching, caching, and state management

---

## ⚙️ Getting Started

Follow these instructions to set up the project on your local machine.

### **Prerequisites**

* [Node.js](https://nodejs.org/) (v18.x or later recommended)
* [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/)
* A local [MongoDB](https://www.mongodb.com/try/download/community) instance or a connection string from MongoDB Atlas

### **Installation**

1.  **Clone the repository**
    ```bash
    git clone 
    cd x-clone.git
    ```

2.  **Set up the Backend**
    ```bash
    # Navigate to the backend directory
    cd backend

    # Install dependencies
    npm install

    # Create a .env file (you can copy .env.example)
    touch .env
    ```

    Add the following environment variables to your `backend/.env` file:
    ```env
    PORT=8000
    MONGO_URI=[Your MongoDB connection string]
    JWT_SECRET=[Your JWT secret key, e.g., a long random string]
    CLOUDINARY_CLOUD_NAME=[Your Cloudinary Cloud Name]
    CLOUDINARY_API_KEY=[Your Cloudinary API Key]
    CLOUDINARY_API_SECRET=[Your Cloudinary API Secret]
    ```

    ```bash
    # Start the backend development server
    npm run dev
    ```
    The backend server will be running on `http://localhost:8000`.

3.  **Set up the Frontend**
    ```bash
    # Navigate to the frontend directory (from the root)
    cd frontend

    # Install dependencies
    npm install

    # Start the frontend development server
    npm run dev
    ```
    The frontend application will be available at `http://localhost:5173` (or another port specified by Vite).

---

## 📁 Project Structure