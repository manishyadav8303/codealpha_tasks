# CodeAlpha Project 1 — Simple URL Shortener

## Requirements
Node.js 18+ and npm.

## Run
```bash
npm install
npm start
```
Server: `http://localhost:3001`

## API
- `POST /api/shorten` JSON body: `{ "url": "https://example.com" }`
- `GET /:code` redirects to the original URL
- `GET /api/urls` lists saved URLs

Data is stored in a local SQLite database (`urls.db`).
