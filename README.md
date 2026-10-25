# CodeAlpha Event Registration System

A responsive event-registration web application built with Node.js, Express, SQLite, HTML, CSS, and JavaScript.

## Features
- Responsive event cards with date, venue, capacity, and seats remaining
- Register for an event using name and email
- Prevent duplicate registrations for the same event/email
- View registrations by email and cancel a booking
- SQLite persistence and REST API endpoints

## Run locally
```bash
npm install
npm start
```
Open http://localhost:3002

## API endpoints
- `GET /api/events` — list events and available seats
- `GET /api/events/:id` — event details
- `POST /api/events` — create an event
- `POST /api/events/:id/register` — register for an event
- `GET /api/registrations?email=...` — find bookings by email
- `DELETE /api/registrations/:id` — cancel a registration
- `GET /api` — API route summary

This is a CodeAlpha internship project. The UI communicates with the Express API; registrations are stored in SQLite.
