# Citizen Engagement System (MVP)

A full-stack web application that allows citizens to submit complaints or feedback on public services. Government institutions can review, respond, and track the status of each complaint through an admin interface.

This is a Minimum Viable Product (MVP) developed to improve transparency, responsiveness, and engagement between citizens and public service providers.

---

## 🚀 Features

### For Citizens
- Submit feedback or complaints via a web form
- Select complaint category (e.g., roads, electricity, health)
- Receive a ticket ID for tracking
- Check the status and response of a complaint

### For Admins
- View all complaints via Django Admin
- Update status (Pending, In Progress, Resolved)
- Respond to complaints with feedback
- Categorize and manage routing (optional extension)

---

## 🛠 Tech Stack

- **Frontend:** React, Bootstrap
- **Backend:** Django, Django REST Framework
- **Database:** SQLite (can be upgraded)
- **Deployment:** Render (Backend) and Netlify (Frontend)

---
## 📁 Project Structure

```bash
├── citizen-engagement-system/
├── backend/
│   ├── gov_feedback/
│   ├── manage.py
├── frontend/
│   ├── public/
│   ├── src/
```

---

## ⚙️ Local Development

### 🔧 Backend Setup

`cd backend`
`python -m venv venv`
`source venv/bin/activate  # or venv\Scripts\activate`
`pip install -r requirements.txt`
`python manage.py migrate`
`python manage.py runserver`

### 🔧 Frontend Setup
`cd frontend`
`npm install`
`npm start`

- Update API base URL in frontend/src/components/ComplaintForm.jsx:
fetch('http://localhost:8000/api/complaints/', ...)

## 🌍 Deployment
🧩 Backend on Render
Create new Web Service

Point to backend/

Use gunicorn gov_feedback.wsgi as start command

💻 Frontend on Netlify

Deploy from frontend/ directory

Set REACT_APP_API_URL in environment variables to backend endpoint

## 📄 License
Maurice Copyright, this code is not allowed to be used anywhere without Maurice permission.



