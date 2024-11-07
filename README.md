Blog Application
================

A simple blog application built using **Express.js**. The application provides features such as creating, editing, and liking blog posts. Users can authenticate, log in, and upload images for their posts. This app uses JWT for authentication and supports file uploads with **multer**.

### Features

*   **User Authentication**: Users can log in with email and password, and authenticate using JWT.
    
*   **Create and Edit Blog Posts**: Users can create new blog posts and edit their existing posts.
    
*   **Like Posts**: Users can like blog posts.
    
*   **Image Upload**: Users can upload images for their blog posts.
    
*   **View Posts**: Users can view all blog posts.
    

### Technologies Used

*   **Express.js**: A minimal web framework for Node.js.
    
*   **EJS**: Embedded JavaScript templating for server side rendering.
    
*   **bcrypt**: Library for hashing passwords.
    
*   **jsonwebtoken (JWT)**: Used for generating and verifying JSON Web Tokens for user authentication.
    
*   **cookie-parser**: Middleware for parsing cookies in requests.
    
*   **multer**: Middleware for handling multipart/form-data for file uploads.
    
*   **crypto**: For generating secure random strings or tokens.
    
*   **path**: Provides utilities for working with file and directory paths.

*   **MongoDB**: NoSQL database for storing user and post data.

*   **Mongoose**:  ODM (Object Data Modeling) library for MongoDB, providing a schema-based solution for interacting with the database.
    

### Installation

1.  Clone the repository to your local machine:
*  **git clone <repositry-url>**

2.  Navigate to Project folder
*  **cd <your-project-folder>**
    
3.  Install the required dependencies:
*  **npm install**

4. Start the application:
*  **npm start**

The app will be available on http://localhost:3000.

### Available Routes

*   **/register**: Register a new user.
    
*   **/login**: Log in an existing user.
    
*   **/profile**: View the profile of the logged-in user.
    
*   **/profile/upload**: Upload a profile image.
    
*   **/edit**: Edit an existing blog post.
    
*   **/logout**: Log out the current user.

### Example Usage

*   **Create a user**: Send a POST request to /register with user details, including a password (which will be hashed using bcrypt).
    
*   **Log in**: Send a GET request to /login with email and password. You will receive a JWT token upon successful authentication.
    
*   **Create a blog post**: Send a POST request to /create with the post content. Optionally, include an image file for the post.
    
*   **Edit a blog post**: Send a POST request to /edit/:postId to update an existing post.
    
*   **Like a post**: Send a POST request to /like/:postId to like a specific post.
    
*   **View posts**: Send a GET request to /posts to see a list of all blog posts.

------------------
### License

This project is licensed under the ISC License.
