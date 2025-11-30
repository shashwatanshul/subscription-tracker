1. High-level Architecture

Your project is a RESTful backend API built in Node.js + Express with:

Express as the HTTP server and routing layer

MongoDB + Mongoose as the database layer

JWT-based auth for user authentication

Arcjet as a security & rate-limiting/bot-detection layer

Upstash Workflows (QStash) to schedule subscription reminder emails

Nodemailer (Gmail SMTP) for sending reminder emails

Conceptually, it looks like this:

Client (Frontend / Postman) → Express API → Middlewares → Controllers → Mongoose Models → MongoDB / External Services (Upstash, Gmail)
