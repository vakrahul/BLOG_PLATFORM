Of course. Here is the complete README.md file formatted in clean, standard Markdown. You can copy and paste this directly into your README.md file on GitHub.

BLOG_PLATFORM
Blog. - A Full-Stack MERN Platform
A modern, full-featured blog platform built with the MERN stack (MongoDB, Express, React, Node.js). This project showcases a complete full-stack application with a professional design, animations, and a rich feature set, including user authentication, post management, local image uploads, a comment system, and more.

Features
This application includes a wide range of modern features:

✅ Full User Authentication: Secure user registration and login with JWT-based session handling.

✅ Complete Blog Post CRUD: Users can create, read, update, and delete their own posts.

✅ Local Image Uploads: Users can upload a featured image for their posts, which is stored locally on the server.

✅ Professional Design: A custom, responsive design with an orange and cream color palette.

✅ Smooth Animations: Integrated animations and page transitions using Framer Motion.

✅ Rich Text Editor: Users can format their blog posts using the react-quill rich text editor.

✅ SEO Compliant: Dynamic page titles and meta descriptions for better search engine visibility using react-helmet-async.

✅ Search Functionality: Users can search for blog posts by title.

✅ Comment System: Logged-in users can leave comments on posts.

✅ Pagination: The main blog feed is paginated for better performance and user experience.

✅ Author Profile Pages: Public profiles for users, showing their bio and a list of their posts.

Tech Stack
Frontend:

React

Redux Toolkit (for state management)

React Router

Axios

SCSS (for styling)

Framer Motion (for animations)

React Icons

Backend:

Node.js

Express

MongoDB with Mongoose

JWT (for authentication)

Multer (for file uploads)

Database:

MongoDB (Local or Atlas)

API Endpoints & Postman
The backend API was developed and tested using Postman. The base URL for all local requests is http://localhost:5001. For Private routes, a Bearer Token obtained from the login endpoint must be included in the Authorization header of the request.

Endpoint	Method	Description	Access
/api/auth/register	POST	Register a new user	Public
/api/auth/login	POST	Authenticate a user & get token	Public
/api/posts	POST	Create a new blog post	Private
/api/posts	GET	Get all posts (paginated)	Public
/api/posts/:id	GET	Get a single post by ID	Public
/api/posts/:id	PUT	Update a post	Private
/api/posts/:id	DELETE	Delete a post	Private
/api/posts/:id/comments	POST	Add a comment to a post	Private
/api/posts/search/:keyword	GET	Search posts by title	Public
/api/posts/user/:userId	GET	Get all posts by a specific user	Public
/api/users/:id	GET	Get a user's public profile	Public
/api/upload	POST	Upload an image file	(Used by protected frontend)
Getting Started
To get a local copy up and running, follow these simple steps.

Prerequisites
Node.js installed on your machine.

MongoDB installed and running locally, or a connection string from MongoDB Atlas.

npm (comes with Node.js).

Installation & Setup
Clone the repository:

Bash
git clone [Link to Your GitHub Repo]
Backend Setup:

Navigate to the backend directory: cd backend

Install NPM packages: npm install

Create a .env file in the backend root and add the following variables:

Code snippet
MONGO_URI=mongodb://localhost:27017/blog
JWT_SECRET=yourjwtsecretkey
PORT=5001
Start the backend server: npm run dev

Your backend will be running at http://localhost:5001

Frontend Setup:

Open a new terminal window.

Navigate to the frontend directory: cd web-frontend

Install NPM packages: npm install

Start the frontend development server: npm run dev

Your frontend will open in your browser at http://localhost:5173
