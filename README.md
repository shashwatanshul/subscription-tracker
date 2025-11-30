# Subscription Tracker Backend

A Node.js + Express backend service for managing user subscriptions and sending automated renewal reminder emails.  
The system uses MongoDB for persistence, JWT for authentication, Upstash Workflows for background scheduling, and Nodemailer for email delivery.

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

## 🏗️ System Architecture Overview

The application follows a **layered REST architecture**:
