Video Learning Platform

A web-based platform for educational video sharing and learning management.
Prerequisites

    Node.js (v14 or higher recommended)
    MongoDB (v4.4 or higher)
    Git

Setup Instructions

    Clone the repository

git clone [your-repository-url]
cd [repository-name]

    Install dependencies

npm install

    MongoDB Setup

    Install MongoDB if not already installed
    Start MongoDB service:
        Windows: MongoDB should be running as a service
        Mac/Linux: sudo service mongod start
    Default MongoDB URL: mongodb://127.0.0.1:27017/

    Environment Variables

# Copy the example environment file
cp .env.example .env

# Edit .env with your values:
# - Set up your email credentials for password reset functionality
# - Adjust MongoDB URI if needed
# - Set your preferred port number

    Start the server

node server.js

The application should now be running at http://localhost:3000 (or your configured port)
Important Notes

    Make sure MongoDB is running before starting the application
    The uploads directory is used for temporary file storage
    Email service requires valid Gmail credentials with App Password
    License keys are managed in db.js - update them as needed

Project Structure

    server.js - Main application entry point
    db.js - Database configuration and operations
    emailService.js - Email service configuration
    HTML files - Frontend pages
    CSS files - Styling
    script.js - Frontend JavaScript

License Keys

The application uses predefined license keys for user registration:

    Student keys: STUDENT_KEY_1, STUDENT_KEY_2
    Teacher keys: TEACHER_KEY_1, TEACHER_KEY_2

Update these in db.js for your specific needs.
Database Collections

    users: Stores user information
    videos: Stores video metadata and content using GridFS

Contributing

    Fork the repository
    Create your feature branch (git checkout -b feature/AmazingFeature)
    Commit your changes (git commit -m 'Add some AmazingFeature')
    Push to the branch (git push origin feature/AmazingFeature)
    Open a Pull Request

