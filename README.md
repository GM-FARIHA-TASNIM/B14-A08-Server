# StudioSpace — Server

StudioSpace Server is a RESTful backend API for managing creative studio listings, user authentication verification, and studio bookings.

## Live Backend

https://studiospace-server-gv67.onrender.com

## Features

- RESTful API architecture.
- MongoDB Atlas database integration.
- Secure JWT verification using Better Auth JWKS.
- Studio listing creation, retrieval, updating, and deletion.
- Studio booking management.
- Protected API endpoints.
- Input validation and error handling.
- CORS configuration for secure frontend communication.

## Technologies Used

- Node.js
- Express.js
- MongoDB
- MongoDB Atlas
- Better Auth
- JOSE
- JWT
- CORS
- dotenv
- Render

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | / | Server status |
| GET | /api/health | Health check |
| GET | /api/studios | Retrieve all studios |
| GET | /api/studios/:id | Retrieve studio details |
| POST | /api/studios | Create a studio |
| PUT | /api/studios/:id | Update a studio |
| DELETE | /api/studios/:id | Delete a studio |
| POST | /api/bookings | Create a booking |

Protected endpoints require a valid Bearer token.

## Local Installation

```bash
git clone https://github.com/GM-FARIHA-TASNIM/B14-A08-Server.git
cd B14-A08-Server
npm install
npm start
```

## Environment Variables

```env
PORT=5000
MONGODB_URI=
CLIENT_URL=
BETTER_AUTH_URL=
```

Configure the database connection variable according to the server configuration.

Never expose database credentials or authentication secrets.

## Client Repository

https://github.com/GM-FARIHA-TASNIM/B14-A08-Client

## Live Website

https://b14-a08-cat-harry.vercel.app/
