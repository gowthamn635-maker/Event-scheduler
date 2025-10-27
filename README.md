🗓 Event Scheduler App (Node.js + Express + MongoDB)
📘 Overview

The Event Scheduler App is a Node.js-based backend application designed to manage and automate event scheduling, reminders, and notifications. It provides RESTful APIs to create, update, cancel, archive, and retrieve events — all from a single endpoint structure. The system ensures efficient event handling with flexible reminder and archiving features.

🚀 Features

Add New Events: Create events with title, description, date, email, and phone notifications.

Get Events: Retrieve all upcoming or archived events.

Update Events: Modify event details or reschedule easily.

Cancel / Archive Events: Mark events as canceled or move them to archive.

Smart Reminders: Supports reminderAt field for scheduling notifications before the event.

MongoDB Integration: All data is stored securely and efficiently using Mongoose.

Error Handling: Includes proper validation and detailed error responses.

Single Endpoint Support: All event-related actions can be handled via one route (/all-in-one) for flexibility.

🧰 Tech Stack

Backend: Node.js, Express.js

Database: MongoDB (Mongoose ORM)

API Testing: Postman

Runtime Environment: Node.js 18+

Language: JavaScript (ES6)

⚙ Installation & Setup

Clone the repository

git clone https://github.com/yourusername/EventScheduler.git
cd EventScheduler


Install dependencies

npm install


Create a .env file and add:

MONGO_URI=mongodb://localhost:27017/eventsdb
PORT=3000


Start the server

node server.js


or (recommended for development)

npx nodemon server.js


Test using Postman

Base URL: http://localhost:3000/all-in-one

Method: POST or GET depending on your action.

🧪 Example Request (Create Event)
POST /all-in-one
{
  "action": "createEvent",
  "data": {
    "title": "Team Meeting",
    "description": "Discuss upcoming project deliverables",
    "eventDate": "2025-11-01T10:00:00Z",
    "reminderAt": "2025-10-31T10:00:00Z",
    "notifyEmail": "team@example.com",
    "notifyPhone": "+919876543210"
  }
}

📦 Folder Structure
EventScheduler/
│
├── config/
│   └── db.js
├── models/
│   └── Event.js
├── routes/
│   └── events.js
├── services/
│   └── scheduler.js
├── server.js
└── package.json

💡 Future Enhancements

Add email/SMS reminder automation.

Add frontend (React or Vue).

Integrate Google Calendar API.

Deploy on Render / Vercel / AWS.

👨‍💻 Author
Gowtham N


Gowtham / Jothimarimuthu K
B.Tech - Artificial Intelligence & Data Science
Anna University
