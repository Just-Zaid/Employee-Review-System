# Employee-Review-System

The provided code outlines the backend setup of an Employee Review System (ERS) using Node.js and the Express framework, following the Model-View-Controller (MVC) architecture. Below is a summary of its key components:

### Key Features:

- **Express Framework:** A minimal and flexible web server for handling requests.
- **EJS with Layouts:** Uses EJS as the templating engine for dynamic HTML pages, with express-ejs-layouts for organizing layouts.
- **MongoDB:** Data storage for user profiles and employee reviews, with session data managed by connect-mongo to persist sessions across server restarts.
- **Session Management:** Handled by express-session, allowing users to remain logged in with session cookies expiring after 100 minutes.
- **Passport.js Authentication:** Utilizes passport-local for username/password authentication, with setAuthenticatedUser middleware for personalized user context.
- **Flash Messages:** Temporary notifications for users using the connect-flash library.
- **Body-Parser:** Middleware to parse incoming request bodies for easy form data handling.
- **Static Assets:** Serves static files like images and CSS from the assets folder.
- **Routes:** Managed in routes/index.js, promoting better organization and maintainability.

### Purpose:  
The system is designed for managing employee reviews, featuring:

- **User Authentication:** Allows employees to log in with credentials.
- **Employee Review:** Enables peer reviews of performance.
- **Flash Notifications:** Provides feedback based on user actions.
- **Session Persistence:** Stores user sessions to survive server restarts.

### Flow:

1. **User Logs In:** Employees or admins log in with their credentials.
2. **Session and Flash Messages:** A session is established, and flash messages communicate success or failure of actions.
3. **Reviewing Employees:** Employees can review one another, with reviews stored in the database.
4. **Rendering Pages:** Dynamic EJS pages are generated, with static assets served appropriately.

### Summary:  
The Employee Review System is a Node.js and Express application that includes user authentication, dynamic rendering with EJS, session management, and MongoDB integration, focusing on employee reviews and enhancing user experience.
