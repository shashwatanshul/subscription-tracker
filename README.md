# Subscription Tracker Backend

A Node.js + Express backend service for managing user subscriptions and sending automated renewal reminder emails. The system uses MongoDB for database, JWT for authentication, Upstash Workflows for background scheduling, and Nodemailer for email delivery.

<img width="1386" height="763" alt="Screenshot 2025-11-30 171008" src="https://github.com/user-attachments/assets/d96162aa-aba4-4a75-9db5-850d199f2a4b" />


## 🏗️ Project Structure

<img width="581" height="783" alt="image" src="https://github.com/user-attachments/assets/469e66ae-ee29-4f5e-92fa-61221abbe8c6" />

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
  - <img width="1037" height="636" alt="image" src="https://github.com/user-attachments/assets/3894eb85-7729-4bf6-a61a-8d30d2298eff" />


- **Robust Database Modeling**
  - Well-structured **MongoDB & Mongoose models**.
  - Clearly defined schemas and relationships between Users and Subscriptions.
  - Automatic calculation of renewal dates and subscription status.
  - <img width="1668" height="915" alt="image" src="https://github.com/user-attachments/assets/823ea4e0-7e3e-4813-ac0b-a7629b35f8fe" />
  - <img width="1664" height="830" alt="image" src="https://github.com/user-attachments/assets/3b25d273-54f7-4251-a972-b7ee99c5b06c" />



- **JWT-Based Authentication**
  - Secure user authentication using **JSON Web Tokens**.
  - Protected routes for:
    - User CRUD operations
    - Subscription creation and management
  - Ownership validation to prevent unauthorized access.
  - <img width="1800" height="832" alt="image" src="https://github.com/user-attachments/assets/b6bc2690-2912-454c-be63-ddc4863de842" />


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


## ✅ Conclusion

This project showcases a well-structured backend system built using Node.js and Express, with a strong focus on security, scalability, and maintainability. By integrating JWT-based authentication, MongoDB with Mongoose for data modeling, Arcjet for application-level security, and Upstash workflows for background processing, the system effectively handles core backend responsibilities.

The architecture follows a clear separation of concerns across routes, controllers, middleware, and services, making the codebase easy to understand and extend. Features like centralized error handling, logging mechanisms, and automated email reminders contribute to a reliable and maintainable system.

Overall, this backend serves as a solid foundation for subscription-based applications and reflects good practices in backend development and system design.



