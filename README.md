# Nyayaag Backend

This is the backend for the Nyayaag platform, built with Node.js, Express, and TypeScript. It provides RESTful APIs for authentication, advocate management, client management, and student features.

## Features

- User authentication (register, login, OTP verification, password reset)
- Advocate profile management and client handling
- Client profile management and advocate search
- Student profile management
- MongoDB for data storage, with session management

## Tech Stack

- Node.js, Express, TypeScript
- MongoDB (via Mongoose)
- Session management with `express-session` and `connect-mongodb-session`
- Environment configuration with `dotenv`

## Getting Started

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Set up environment variables:**
   Create a `.env` file in the root with:
   ```
   PORT=3000
   MONGODB_URI=your_mongodb_connection_string
   SESSION_SECRET=your_session_secret
   COLLECTION_NAME=sessions
   ```

3. **Run in development:**
   ```bash
   npm run start:dev
   ```

4. **Build and run in production:**
   ```bash
   npm run start
   ```

## API Endpoints

### Auth (`/auth`)
- `POST /register` — Register a new user
- `POST /login` — Login
- `POST /verifyOTP` — Verify OTP
- `POST /resendOTPVerification` — Resend OTP
- `POST /forgotPassword` — Forgot password
- `POST /resetPassword` — Reset password

### Advocate (`/advocate`)
- `POST /updatePersonalDetails`
- `POST /updateAdvocateBarDetails`
- `POST /addclient`
- `POST /caseReminder`
- `POST /profile`
- `POST /viewClients`

### Client (`/client`)
- `GET /` — Test route
- `POST /update`
- `POST /getAdvocate`

### Student (`/student`)
- `POST /update`

## Scripts

- `npm run start:dev` — Start in development mode
- `npm run start` — Build and start in production
- `npm run lint` — Lint code

---

Let me know if you want to add more details or usage examples!
