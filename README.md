# ThreatLens – Digital Identity & Threat Exposure Analyzer

ThreatLens is a cybersecurity web application that helps users analyze how exposed their digital identity is on the internet. It allows users to scan their email for known data breaches and check whether a URL is malicious using real threat intelligence APIs.

The goal of this project is to provide a simple security dashboard that gives users quick insights into their digital risk and suggests actions to improve their online safety.

---

## Features

Email Breach Scanner
Checks whether an email address has appeared in known data breaches using the RapidAPI Breach Directory service.

Malicious URL Scanner
Analyzes suspicious links using the VirusTotal threat intelligence platform to determine whether a URL is flagged by security engines.

Security Dashboard
Displays results in a cybersecurity-themed dashboard showing scan results and risk indicators.

User Friendly Interface
Modern dark themed UI with Tailwind CSS and animations.

Risk Awareness
Provides security recommendations based on scan results.

---

## Tech Stack

Frontend

* React (Vite)
* Tailwind CSS
* Axios
* Framer Motion
* React Router

Backend

* Node.js
* Express.js
* Axios
* dotenv
* cors

APIs Used

* RapidAPI Breach Directory
* VirusTotal

---

## Project Structure

ThreatLens

frontend
src
components
pages
Home.jsx
Scan.jsx
Dashboard.jsx
services
App.jsx
main.jsx

backend
routes
emailRoute.js
urlRoute.js
services
emailService.js
urlService.js
server.js
.env

---

## How It Works

1. The user enters an email or URL on the scan page.
2. The React frontend sends the request to the Node.js backend.
3. The backend communicates with external threat intelligence APIs.
4. The results are processed and returned to the frontend.
5. The dashboard displays the risk analysis and recommendations.

System Flow

User → React Frontend → Express Backend → Security APIs → Results Dashboard

---

## Installation

Clone the repository

git clone https://github.com/yourusername/threatlens.git

Navigate into the project folder

cd threatlens

---

## Backend Setup

Navigate to the backend folder

cd backend

Install dependencies

npm install

Create a .env file and add your API keys

RAPIDAPI_KEY=your_rapidapi_key
VIRUSTOTAL_API_KEY=your_virustotal_key
PORT=5000

Start the backend server

node server.js

---

## Frontend Setup

Navigate to the frontend folder

cd frontend

Install dependencies

npm install

Start the development server

npm run dev

---

## Usage

1. Open the application in your browser.
2. Navigate to the scan page.
3. Enter an email to check if it has been involved in a data breach.
4. Enter a URL to analyze whether it is malicious.
5. View the results in the dashboard along with security recommendations.

---

## Security Recommendations

If your email appears in a breach:

* Change your password immediately.
* Enable two-factor authentication.
* Avoid reusing passwords across different sites.

If a URL is flagged as malicious:

* Do not visit the website.
* Avoid entering personal information.
* Report the link if it appears to be phishing.

---

## Future Improvements

Password leak scanner using Pwned Passwords API
Username exposure scanner (OSINT based)
Advanced risk scoring system
More threat intelligence integrations
Interactive charts and analytics

---

## Disclaimer

ThreatLens is intended for educational and demonstration purposes only. The results are based on publicly available threat intelligence APIs and should not be considered a complete security assessment.

---

