#
 FLIPR Full Stack Assignment

This is a complete Full Stack application (MERN Stack) built for the Flipr placement task. It consists of a Landing Page for a Real Estate company and an Admin Panel to manage its content.

## Project Structure
- `client/`: Frontend application using React, Vite, and TailwindCSS.
- `server/`: Backend API using Node.js, Express, and MongoDB.

## Prerequisites
Before you begin, ensure you have the following installed on your system:
- **Node.js**: [Download Here](https://nodejs.org/) (Version 14 or higher)
- **MongoDB**: [Download Here](https://www.mongodb.com/try/download/community) (Or use a Cloud Atlas account)
- **Git**: [Download Here](https://git-scm.com/)

## Step-by-Step Setup Guide

### 1. Database Setup
Ensure your MongoDB service is running locally.
- If you installed MongoDB Compass or Community Server, it usually runs at `mongodb://localhost:27017`.
- If you are using MongoDB Atlas, get your connection string (e.g., `mongodb+srv://<user>:<password>@cluster...`).

### 2. Setup Backend (Server)
1.  Open your terminal.
2.  Navigate to the `server` directory:
    ```bash
    cd server
    ```
3.  Install dependencies:
    ```bash
    npm install
    ```
4.  Configure Environment Variables:
    - The project comes with a `.env` file pre-configured for local MongoDB.
    - If you need to change it, open `.env` and update `MONGO_URI`.

### 3. Setup Frontend (Client)
1.  Open a new terminal (or navigate back to root).
2.  Navigate to the `client` directory:
    ```bash
    cd client
    ```
3.  Install dependencies:
    ```bash
    npm install
    ```

### 4. Running the Application
You can run both Client and Server with a single command from the project **root** directory.

1.  Navigate to the root directory `fullstack-assignment`:
    ```bash
    npm install  # Installs the 'concurrently' tool
    npm start
    ```
2.  The application will open:
    - **Frontend**: [http://localhost:5173](http://localhost:5173)
    - **Backend**: [http://localhost:5000](http://localhost:5000)

### 5. Accessing Features
- **Landing Page**: Visit the homepage to see the Hero, About, Projects, and Clients sections.
- **Admin Panel**: Click the **ADMIN** link in the Navbar or visit [http://localhost:5173/admin](http://localhost:5173/admin).
  - Manage Projects (Add images/descriptions)
  - Manage Happy Clients (Add testimonials)
  - View Contact Form Submissions
  - View Newsletter Subscribers



## Evaluation Criteria Met
- **Functionality**: Full CRUD for Projects/Clients, Contact Form submission, Newsletter.
- **Code Quality**: Clean architecture with Controller/Model separation.
- **Design**: Pixel-perfect adherence to reference images using TailwindCSS.
- **Usability**: Responsive layout and easy-to-use Admin Panel.
- **Bonus**: Image cropping/resizing implemented on backend using `sharp`.
