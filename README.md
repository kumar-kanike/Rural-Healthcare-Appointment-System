# Rural Healthcare Appointment System

A React + Node.js/Express + MongoDB MVP for rural patients to request appointments and keep a private appointment history.

## Features
- Email/password registration and login with bcrypt + JWT.
- Submit appointment requests with patient, contact, doctor/clinic, date, village and visit reason.
- Private appointment history scoped to the signed-in user.
- MongoDB Atlas persistence and responsive React interface.

## Stack
React, Vite, Node.js, Express, MongoDB Atlas, Mongoose.

## Database
`rural_healthcare_db` — collections: `users`, `doctors`, `appointments`, `medicalRecords`.

## Run
Create an Atlas database user and allow the backend host IP. Copy `backend/.env.example` to `backend/.env`; set `MONGODB_URI` and a random 32+ character `JWT_SECRET`. Run `cd backend && npm install && npm run dev`; in a second terminal run `cd frontend && npm install && npm run dev`. Open port 5173.

## Production gap
This MVP does not verify doctors, provide telemedicine, or store clinical records. Add provider verification, consent, privacy controls, appointment reminders, secure medical-record handling and audit logs before handling real patient data.
