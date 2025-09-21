# **BLOG_PLATFORM**

**Blog – A Full-Stack MERN Platform**

A modern, full-featured blog platform built with the **MERN stack (MongoDB, Express, React, Node.js)**.  
This project showcases a complete full-stack application with a **professional design, animations, and a rich feature set**, including **user authentication, post management, local image uploads, a comment system, and more.**

---

## **✨ Features**

This application includes a wide range of modern features:

- ✅ **Full User Authentication**: Secure user registration and login with JWT-based session handling.  
- ✅ **Complete Blog Post CRUD**: Users can create, read, update, and delete their own posts.  
- ✅ **Local Image Uploads**: Users can upload a featured image for their posts, which is stored locally on the server.  
- ✅ **Professional Design**: A custom, responsive design with an orange and cream color palette.  
- ✅ **Smooth Animations**: Integrated animations and page transitions using **Framer Motion**.  
- ✅ **Rich Text Editor**: Users can format their blog posts using the **react-quill** rich text editor.  
- ✅ **SEO Compliant**: Dynamic page titles and meta descriptions for better search engine visibility using **react-helmet-async**.  
- ✅ **Search Functionality**: Users can search for blog posts by title.  
- ✅ **Comment System**: Logged-in users can leave comments on posts.  
- ✅ **Pagination**: The main blog feed is paginated for better performance and user experience.  
- ✅ **Author Profile Pages**: Public profiles for users, showing their bio and a list of their posts.  

---

## **🛠 Tech Stack**

### **Frontend**
- React  
- Redux Toolkit (for state management)  
- React Router  
- Axios  
- SCSS (for styling)  
- Framer Motion (for animations)  
- React Icons  

### **Backend**
- Node.js  
- Express  
- MongoDB with Mongoose  
- JWT (for authentication)  
- Multer (for file uploads)  

### **Database**
- MongoDB (Local or Atlas)
- 
For **Private routes**, a **Bearer Token** obtained from the login endpoint must be included in the **Authorization header** of the request.

| **Endpoint** | **Method** | **Description** | **Access** |
|--------------|------------|-----------------|------------|
| `/api/auth/register` | POST | Register a new user | Public |
| `/api/auth/login` | POST | Authenticate a user & get token | Public |
| `/api/posts` | POST | Create a new blog post | Private |
| `/api/posts` | GET | Get all posts (paginated) | Public |
| `/api/posts/:id` | GET | Get a single post by ID | Public |
| `/api/posts/:id` | PUT | Update a post | Private |
| `/api/posts/:id` | DELETE | Delete a post | Private |
| `/api/posts/:id/comments` | POST | Add a comment to a post | Private |
| `/api/posts/search/:keyword` | GET | Search posts by title | Public |
| `/api/posts/user/:userId` | GET | Get all posts by a specific user | Public |
| `/api/users/:id` | GET | Get a user's public profile | Public |
| `/api/upload` | POST | Upload an image file (Used by protected frontend) | Private |

---

## **🚀 Getting Started**

Follow these steps to set up a local development environment:

### **Prerequisites**
- Install [Node.js](https://nodejs.org/) on your machine.  

### **Clone the Repository**
```bash
git clone https://github.com/vakrahul/Blog-platform.git
cd Blog-platform

cd web-frontend
npm install
cd backend
npm install

