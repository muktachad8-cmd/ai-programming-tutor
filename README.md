# AI Programming Tutor

A portfolio-ready full-stack AI programming tutor built with React, TypeScript, Node.js, Express, PostgreSQL/Prisma, and an optional OpenAI-compatible AI provider.

## Features
- React + TypeScript responsive dashboard
- Node.js + Express REST API
- PostgreSQL with Prisma ORM
- User registration/login with JWT
- AI tutor endpoint with mock fallback
- Practice problems and progress tracking
- Clean project structure for future microservices/AWS expansion

## Run locally
1. Copy `server/.env.example` to `server/.env` and set `DATABASE_URL` and `JWT_SECRET`.
2. Optional: set `AI_API_KEY` and `AI_BASE_URL` for an OpenAI-compatible provider. If omitted, the tutor uses a safe local mock response.
3. Start PostgreSQL with Docker:
   `docker compose up -d db`
4. Install dependencies:
   `cd server && npm install && npx prisma migrate dev --name init && npm run seed && npm run dev`
5. In another terminal:
   `cd client && npm install && npm run dev`
6. Open the Vite URL shown in the terminal.

## Demo account
After seeding: `demo@aitutor.local` / `Demo1234!`

## Portfolio notes
Replace the mock AI provider with your chosen model provider, add tests, CI/CD, AWS deployment, and screenshots before presenting this project to employers.
