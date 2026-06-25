# Setup Guide for environment variables & API Keys

This guide contains the prompt and reference configuration that you can copy and paste directly into Claude to be guided step-by-step through setting up all 5 service integrations.

---

## 📋 Copy-Paste Prompt for Claude

Copy the entire block below and paste it into a new Claude chat:

```markdown
I have a Node.js (backend) and Vite (frontend) web application called "Talent IQ / Interview Platform". I need to configure the environment variables for 5 services. 

Please guide me step-by-step, **one service at a time**, through setting up each integration. Give me the steps for the first service, then wait for me to tell you "next" or "done" before providing the steps for the next service.

For each service, tell me:
1. Where to sign up/log in.
2. Exactly how to find the specific keys in their dashboard.
3. What values to fill into my `.env` files (both backend and frontend).

Here is my project's environment variable configuration:

### 1. Clerk Authentication
- Backend needs:
  CLERK_PUBLISHABLE_KEY=
  CLERK_SECRET_KEY=
- Frontend needs:
  VITE_CLERK_PUBLISHABLE_KEY= (Must match backend CLERK_PUBLISHABLE_KEY)

### 2. Stream.io (Video Call & Chat)
- Backend needs:
  STREAM_API_KEY=
  STREAM_API_SECRET=
- Frontend needs:
  VITE_STREAM_API_KEY= (Must match backend STREAM_API_KEY)

### 3. Inngest (Background Job Queue)
- Backend needs:
  INNGEST_EVENT_KEY=
  INNGEST_SIGNING_KEY=
- Note: Mention if we can run locally without cloud keys during development.

### 4. MongoDB Database
- Backend needs:
  DB_URL= (MongoDB connection string)

### 5. Application Host Settings
- Backend needs:
  PORT=3000
  NODE_ENV=development
  CLIENT_URL=http://localhost:5173
- Frontend needs:
  VITE_API_URL=http://localhost:3000/api

Let's start with service "1. Clerk Authentication". Please give me the steps to set it up!
```

---

## 🛠️ Reference Files

Your project has the following template files for environment variables:
- **Backend Environment Template:** [backend/.env.example](file:///c:/Users/hksha/OneDrive/Desktop/talent-IQ-master/backend/.env.example)
- **Frontend Environment Template:** [frontend/.env.example](file:///c:/Users/hksha/OneDrive/Desktop/talent-IQ-master/frontend/.env.example)

When you are ready, create the following `.env` files in your project and fill them with the keys you get:
1. `backend/.env`
2. `frontend/.env`
