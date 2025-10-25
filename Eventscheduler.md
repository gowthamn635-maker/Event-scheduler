# Event Scheduler (Node.js + Express + MongoDB + node-cron)

## Requirements
- Node.js 16+
- MongoDB (local or URI)
- (Optional) Email SMTP credentials (Gmail app password or SMTP)
- (Optional) Twilio account for SMS

## Setup
1. Clone or copy project files into a folder `event-scheduler`.
2. `cd event-scheduler`
3. `npm install`
4. Copy `.env.example` to `.env` and fill values (especially `MONGODB_URI`, email & Twilio if you want real notifications).
5. Start MongoDB locally, or provide a cloud URI.
6. Run:
