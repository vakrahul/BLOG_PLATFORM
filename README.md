"# BLOG_PLATFORM" 
Blog. - A Full-Stack MERN Platform
A modern, full-featured blog platform built with the MERN stack (MongoDB, Express, React, Node.js). This project showcases a complete full-stack application with a professional design, animations, and a rich feature set, including user authentication, post management, local image uploads, a comment system, and more.

________________________________________
Features
This application includes a wide range of modern features:
•	✅ Full User Authentication: Secure user registration and login with JWT-based session handling.
•	✅ Complete Blog Post CRUD: Users can create, read, update, and delete their own posts.
•	✅ Local Image Uploads: Users can upload a featured image for their posts, which is stored locally on the server.
•	✅ Professional Design: A custom, responsive design with an orange and cream color palette.
•	✅ Smooth Animations: Integrated animations and page transitions using Framer Motion.
•	✅ Rich Text Editor: Users can format their blog posts using the react-quill rich text editor.
•	✅ SEO Compliant: Dynamic page titles and meta descriptions for better search engine visibility using react-helmet-async.
•	✅ Search Functionality: Users can search for blog posts by title.
•	✅ Comment System: Logged-in users can leave comments on posts.
•	✅ Pagination: The main blog feed is paginated for better performance and user experience.
•	✅ Author Profile Pages: Public profiles for users, showing their bio and a list of their posts.
________________________________________
Tech Stack
•	Frontend:
•	React
•	Redux Toolkit (for state management)
•	React Router
•	Axios
•	SCSS (for styling)
•	Framer Motion (for animations)
•	React Icons
•	Backend:
•	Node.js
•	Express
•	MongoDB with Mongoose
•	JWT (for authentication)
•	Multer (for file uploads)
•	Database:
•	MongoDB (Local or Atlas)
________________________________________
API Endpoints & Postman
The backend API was developed and tested using Postman. The base URL for all local requests is http://localhost:5001.
For Private routes, a Bearer Token obtained from the login endpoint must be included in the Authorization header of the request.
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
________________________________________
Getting Started
To get a local copy up and running, follow these simple steps.
Prerequisites
•	Node.js installed on your machine.
•	MongoDB installed and running locally, or a connection string from MongoDB Atlas.
•	npm (comes with Node.js).
Installation & Setup
1.	Clone the repository:
Bash
git clone [Link to Your GitHub Repo]
2.	Backend Setup:
•	Navigate to the backend directory: cd backend
•	Install NPM packages: npm install
•	Create a .env file in the backend root and add the following variables:
Code snippet
MONGO_URI=mongodb://localhost:27017/blog
JWT_SECRET=yourjwtsecretkey
PORT=5001
•	Start the backend server: npm run dev
•	Your backend will be running at http://localhost:5001
3.	Frontend Setup:
•	Open a new terminal window.
•	Navigate to the frontend directory: cd web-frontend
•	Install NPM packages: npm install
•	Start the frontend development server: npm run dev
•	Your frontend will open in your browser at http://localhost:5173
________________________________________
Leveraging AI in Development (Assignment Requirement)
As per the assignment requirements, AI tools were extensively used throughout the development process to improve efficiency, solve complex problems, and implement professional practices.
Prompting Techniques Used
My process involved several key prompting techniques:
1.	Role-Based Prompting: "Act as a senior full-stack developer. I need to build a blog application. What is a professional project structure?"
2.	Boilerplate Generation: "Generate the full code for a Node.js Express server with a Mongoose connection." or "Create a Redux Toolkit slice for user authentication."
3.	Code Refactoring & Explanation: "Here is my React component. Can you refactor it to include loading and error states?" or "Explain this useEffect hook line-by-line."
4.	Debugging & Error Analysis: "I'm getting the error net::ERR_CONNECTION_REFUSED. Here is my console log. What are the likely causes and how do I fix it?"
How AI Helped
•	Project Scaffolding: AI helped generate the initial file structure and boilerplate code for the backend server, frontend project setup, and Redux store.
•	Feature Implementation: It provided the complete code for complex features like JWT authentication middleware, Redux async thunks for API calls, and the logic for the rich text editor and local image uploads.
•	Debugging: AI was instrumental in diagnosing and fixing a wide range of errors, from simple typos (redux-react vs react-redux) to complex issues like version conflicts (react-quill with React 19) and state management bugs (infinite loops in useEffect).
•	Design and Styling: AI provided the complete SCSS code for the professional orange and cream theme, including responsive design elements and animations.
Challenges Faced
•	Version Conflicts: A major challenge was the incompatibility between react-quill and the latest version of React. AI helped diagnose the findDOMNode error and suggested the solution of downgrading React to a compatible version.
•	State Management Bugs: An infinite loop was created by an incorrectly configured useEffect dependency array. AI helped identify the logical flaw and provided the corrected code to fix the loop. Another subtle bug where success notifications fired at the wrong time was fixed by introducing a more specific state flag (postCreated), a solution suggested and implemented by AI.
•	API Connection Issues: Persistent ERR_CONNECTION_REFUSED errors were solved by a systematic, AI-guided environmental check (verifying server status, checking for firewalls, etc.).
