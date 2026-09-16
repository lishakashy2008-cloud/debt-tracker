# DEBT — Productivity RPG (Full Stack)

This version adds a real backend and SQLite database.

## Features
- Express.js backend
- SQLite database (`data/debt_rpg.db`)
- User signup/login stored in database
- Passwords hashed with bcrypt
- JWT login session
- Tasks, XP, level, boss HP and battle logs saved per user
- Frontend calls `/api/*` instead of browser `localStorage` for game data

## Run on a computer

1. Install Node.js 18+.
2. Open a terminal in this folder.
3. Run:
   ```bash
   npm install
   npm start
   ```
4. Open `http://localhost:3000`

The SQLite database is created automatically at `data/debt_rpg.db`.

## Production note
Set a strong `JWT_SECRET` environment variable before deploying. For a public deployment, also use HTTPS and a proper session/token strategy.
