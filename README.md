# AI Assistant Backend

REST API backend for an AI-based personal assistant, built with Express and MongoDB.

## Features

- User signup/login with hashed passwords (bcryptjs) and token-based auth
- Per-user data storage: each user's assistant data is kept in its own Mongoose model
- Encryption and hashing utilities for sensitive fields (`utils/encrypt.js`, `utils/hash.js`)
- Environment-based config with dotenv

## Structure

- `server.js` - app entry point
- `config/db.js` - MongoDB connection
- `models/` - `User` and `UserData` Mongoose schemas
- `controllers/` - request handlers for auth and user data
- `routes/` - API route definitions
- `utils/` - encryption and hashing helpers

## Run it

```
npm install
cp .env.example .env   # set MONGO_URI and your secret
npm run dev            # nodemon
# or
npm start
```

## Stack

Node.js, Express, MongoDB (Mongoose), bcryptjs
