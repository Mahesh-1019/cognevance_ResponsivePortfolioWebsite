# Responsive Portfolio Website

A responsive personal portfolio website built for the Cognevance Technologies Full Stack Web Developer internship Task 1.

## Features
- Responsive portfolio UI
- About, Skills, Projects and Contact sections
- Mobile navigation
- Scroll animations and reveal effects
- Contact form with frontend validation
- Express REST API for contact messages
- MongoDB/Mongoose persistence
- CORS and environment-variable configuration
- Clean frontend/backend folder structure

## Tech Stack
- Frontend: HTML5, CSS3, JavaScript
- Backend: Node.js, Express.js
- Database: MongoDB + Mongoose

## Project Structure
```text
cognevance_ResponsivePortfolioWebsite/
├── client/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── server/
│   ├── models/
│   │   └── Contact.js
│   ├── .env.example
│   ├── index.js
│   └── package.json
├── docs/
│   ├── database-schema.md
│   ├── api-documentation.md
│   ├── screenshots/README.md
│   └── project-report.md
├── .gitignore
└── README.md
```

## Run Locally

### 1. Backend
```bash
cd server
npm install
cp .env.example .env
npm start
```

The API runs on `http://localhost:5000`.

### 2. Frontend
Open `client/index.html` with a local static server. For example:
```bash
cd client
python3 -m http.server 5500
```
Then open `http://localhost:5500`.

If the backend URL is different, edit `API_BASE_URL` near the top of `client/script.js`.

## Environment Variables
Create `server/.env` from `.env.example`:
```env
PORT=5000
MONGODB_URI=mongodb://127.0.0.1:27017/cognevance_portfolio
CLIENT_URL=http://localhost:5500
```

For MongoDB Atlas, replace `MONGODB_URI` with your Atlas connection string.

## API
- `GET /api/health` - API health check
- `POST /api/contact` - Save a contact message
- `GET /api/contact` - View saved messages (demo/admin development endpoint)

See `docs/api-documentation.md` for request/response details.

## Deployment
Recommended:
- Frontend: Vercel or Netlify
- Backend: Render or Railway
- Database: MongoDB Atlas

Update the frontend API URL after deploying the backend.

## Internship Deliverables
- Frontend source code
- Backend source code
- Database setup
- Screenshots/demo
- Deployment links
- GitHub repository

> Replace the placeholder contact details, social links and project links with your own before final submission.
