# Subscription Tracker Backend

A Node.js + Express backend service for managing user subscriptions and sending automated renewal reminder emails.  
The system uses MongoDB for persistence, JWT for authentication, Upstash Workflows for background scheduling, and Nodemailer for email delivery.

<img width="1386" height="763" alt="image" src="https://github.com/user-attachments/assets/d55dd90e-d62d-4e2b-bc87-50c1196cef60" />


---

## 🚀 Tech Stack

- **Node.js** – Runtime environment
- **Express.js** – REST API framework
- **MongoDB + Mongoose** – Database and ODM
- **JWT (JSON Web Token)** – Authentication
- **Arcjet** – Security (rate limiting, bot detection)
- **Upstash Workflows (QStash)** – Background job scheduling
- **Nodemailer (Gmail SMTP)** – Email notifications

---

## ✨ Features

- **Advanced Rate Limiting & Bot Protection**
  - Integrated **Arcjet** for global protection against abuse.
  - Prevents bots, applies rate limits, and secures all API endpoints at the middleware level.

- **Robust Database Modeling**
  - Well-structured **MongoDB & Mongoose models**.
  - Clearly defined schemas and relationships between Users and Subscriptions.
  - Automatic calculation of renewal dates and subscription status.

- **JWT-Based Authentication**
  - Secure user authentication using **JSON Web Tokens**.
  - Protected routes for:
    - User CRUD operations
    - Subscription creation and management
  - Ownership validation to prevent unauthorized access.

- **Global Error Handling**
  - Centralized error middleware for consistent error responses.
  - Handles validation errors, database errors, and application errors gracefully.
  - Cleaner controllers with predictable error flow.

- **Logging & Debugging Mechanisms**
  - Structured logging for API activity and server events.
  - Helpful console outputs for development and monitoring.
  - Centralized handling improves debuggability in production.

- **Automated Email Reminders**
  - Smart subscription renewal reminders using **Upstash Workflows (QStash)**.
  - Background scheduling for reminder emails:
    - 7, 5, 2, and 1 day(s) before renewal.
  - Automated email delivery using **Nodemailer** with dynamic templates.


## 🏗️ Project Structure

<img width="581" height="783" alt="image" src="https://github.com/user-attachments/assets/469e66ae-ee29-4f5e-92fa-61221abbe8c6" />


