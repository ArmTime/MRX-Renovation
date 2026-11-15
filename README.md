# MRX Renovation

Responsive home-renovation planner for desktop and mobile. Includes Armenian, Russian and English UI, local data storage, budget tracking, rooms, materials calculator, task planner, PWA install support, and an optional AI design endpoint.

## Requirements
- Node.js 18 or newer
- Internet connection for first-time package installation and optional AI requests

## Run on Windows 11
1. Install Node.js LTS from https://nodejs.org/.
2. Extract this project folder.
3. Open PowerShell in the `mrx-renovation` folder.
4. Run `npm install` and then `npm start`.
5. Open http://localhost:3000 in Chrome or Edge.

## Enable AI designer
Copy `.env.example` to `.env` and set `OPENAI_API_KEY`. Keep the key on the server; never put it in frontend code or GitHub. API usage may incur charges.

## Deploy with Render
This project includes `render.yaml`. In Render choose New → Blueprint, connect this repository, and deploy. Add `OPENAI_API_KEY` as a secret environment variable only if you want AI design enabled.

## Data and privacy
Project data is stored in each browser's localStorage and is not automatically synchronized between devices. Add a database and authentication before using this as a multi-user production service.
