﻿# chesswebgame
 
A full-featured Chess App that integrates modern backend security and architecture techniques using Node.js and Express. This app doesn’t just let users play chess — it also handles user authentication, route protection, and secure data handling using tools like bcrypt, JWT tokens, and custom middleware.

At its core, the app is divided into clear and organized routes such as /auth for login/signup and /game for playing. These routes are handled through Express’s routing system to keep the logic modular and scalable.

To ensure user passwords are never stored in plain text, we’ve used bcrypt, which hashes the passwords before saving them to your database. This adds a strong layer of protection against data breaches. During login, bcrypt also verifies the password by comparing the hash with the user’s input.

For authentication, we’ve implemented JWT (JSON Web Tokens). When a user logs in, your app creates a token signed with a secret key. This token is sent to the client and must be included in future requests to protected endpoints (like making a move in the chess game). This ensures that only authenticated users can access game logic.


🔑 Key Features we've Implemented:

✅ Secure Password Hashing with bcrypt

✅ User Authentication using JWT tokens

✅ Protected Routes with custom middleware

✅ Modular Routing for cleaner code structure

✅ Environment Variables for secure token handling (.env file)

✅ Organized MVC-style structure (routes/, controllers/, middleware/)
