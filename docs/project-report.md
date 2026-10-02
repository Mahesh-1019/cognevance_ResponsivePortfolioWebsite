# Responsive Portfolio Website - Project Report

## 1. Introduction
This project is a responsive personal portfolio website developed for the Cognevance Technologies Full Stack Web Developer internship, Level 1 Task 1.

## 2. Objectives
- Build a responsive personal website.
- Create About, Skills, Projects and Contact sections.
- Add responsive navigation and animations.
- Connect the contact form to a backend API.
- Store submitted messages in MongoDB.
- Prepare the application for deployment.

## 3. Architecture
Browser → HTML/CSS/JavaScript frontend → Express REST API → Mongoose → MongoDB.

## 4. Functional Workflow
1. Visitor opens the portfolio.
2. Visitor navigates through the responsive sections.
3. Visitor fills the contact form.
4. Frontend validates required fields.
5. Frontend sends JSON to `POST /api/contact`.
6. Express validates the request.
7. Mongoose stores the message in MongoDB.
8. API returns a success or error response.

## 5. Technologies
HTML5, CSS3, JavaScript, Node.js, Express.js, MongoDB and Mongoose.

## 6. Testing Checklist
- [ ] Desktop layout
- [ ] Mobile layout
- [ ] Navigation menu
- [ ] Section scrolling
- [ ] Scroll reveal animations
- [ ] Required field validation
- [ ] Invalid email validation
- [ ] Contact API success
- [ ] MongoDB persistence
- [ ] API health check
- [ ] Deployment

## 7. Deployment
Recommended deployment:
- Frontend: Vercel/Netlify
- Backend: Render/Railway
- Database: MongoDB Atlas

## 8. Screenshots
Add final screenshots to `docs/screenshots/` after running the application.
