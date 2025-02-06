# Express.js Authentication Project






This project demonstrates a simple authentication mechanism using **Express.js**. It showcases my understanding of backend development, middleware usage, and handling HTTP requests and responses. Below is a detailed overview of the project, the technologies used, and how to run it.

---

## Technologies Used

- **Express.js**: A fast, unopinionated, and minimalist web framework for Node.js.
- **Body-parser**: Middleware to parse incoming request bodies.
- **Node.js**: JavaScript runtime used to build scalable network applications.
- **Postman**: Used for testing API endpoints and verifying the functionality of the authentication system.

---

## Project Overview

This project implements a basic password-based authentication system. The user is required to enter a password (`ILoveProgramming`) to access a secret page. If the password is correct, the user is redirected to the secret page; otherwise, they are redirected back to the home page.

### Key Features:
1. **Middleware for Password Validation**: A custom middleware (`passwordCheck`) is used to validate the password submitted by the user.
2. **Static File Serving**: The project serves static HTML files (`index.html` and `secret.html`) using Express.js.
3. **Form Handling**: The app handles form submissions using `body-parser` to extract data from the request body.

---

## How to Run the Project

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
2. **Install Dependencies:**
    Make sure you have Node.js installed. Then, run:
    ```bash
    npm install
3. **Run the application**
   ```bash
   node index.js
4. **Access the Application:**
    Open your browser and navigate to http://localhost:3000. Enter the password ILoveProgramming to access the secret page.

---

## Testing with Postman

I used **Postman** to test the application's functionality. Here's how you can test it:

### GET Request:
- **URL**: `http://localhost:3000/`
- **Method**: `GET`
- **Description**: This will return the `index.html` file.

### POST Request:
- **URL**: `http://localhost:3000/check`
- **Method**: `POST`
- **Body**: `x-www-form-urlencoded`
- **Key**: `password`
- **Value**: `ILoveProgramming`
- **Description**: If the password is correct, the response will be the `secret.html` file. Otherwise, you'll be redirected to the home page.
