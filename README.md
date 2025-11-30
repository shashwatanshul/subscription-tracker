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

## 🏗️ System Architecture Overview

The application follows a **layered REST architecture**:

<img width="575" height="813" alt="image" src="https://github.com/user-attachments/assets/f52895b1-2911-4e9b-bf35-8a45ca434e9f" />

