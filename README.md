# Chatty 💬

A full-stack real-time chat application. This README covers the backend setup and structure.

---

## Tech Stack

- **Runtime:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB (via Mongoose)
- **Auth:** JWT-based authentication
- **Environment:** dotenv

---

## Project Structure

```
├── index.js                  # Entry point
├── lib/
│   └── db.js                 # MongoDB connection
├── routes/
│   └── auth.route.js         # Auth routes
├── controllers/
│   └── auth.controller.js    # Auth logic
├── models/
│   └── user.model.js         # User schema
└── .env                      # Environment variables
```

---

## Getting Started

### Prerequisites

- Node.js (v18+)
- MongoDB instance (local or Atlas)

### Installation

1. **Clone the repository**

```bash
git clone https://github.com/your-username/chatty.git
cd chatty
```

2. **Install dependencies**

```bash
npm install
```

3. **Set up environment variables**

Create a `.env` file in the root directory:

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

4. **Start the server**

```bash
# Development
npm run dev

# Production
npm start
```

The server will start on the port defined in your `.env` file.

---

## API Endpoints

### Auth Routes — `/api/auth`

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/signup` | Register a new user |
| POST | `/api/auth/login` | Login an existing user |
| POST | `/api/auth/logout` | Logout the current user |

---

## Environment Variables

| Variable | Description |
|----------|-------------|
| `PORT` | Port the server runs on |
| `MONGODB_URI` | MongoDB connection string |
| `JWT_SECRET` | Secret key for signing JWT tokens |

---

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

## License

[MIT](LICENSE)
