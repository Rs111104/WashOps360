DryClean

Pickup & Delivery Garment Care — simple, reliable, and efficient.

Overview

DryClean is a prototype service that simplifies the dry-cleaning experience.
Customers can schedule pickups, track the cleaning process, and get timely delivery updates.
Admins can manage orders, update statuses, and send automated notifications.

This project demonstrates product thinking, full-stack development, and integration with real-world APIs.

Features

📦 Order placement with pickup scheduling

🗂️ Admin dashboard for managing and updating orders

📲 Automated customer notifications (SMS/WhatsApp via Twilio)

✅ Item checklist and quality control notes

🗃️ Lightweight database (SQLite) for easy local setup

Tech Stack

Backend: Python (Flask)

Database: SQLite (easily portable to PostgreSQL)

Messaging: Twilio (WhatsApp/SMS integration)

Tools: ngrok (for local webhook testing)

Quickstart

Clone this repository:
git clone https://github.com/your-username/dryclean.git
cd dryclean

Create a virtual environment and install dependencies:
python -m venv venv
source venv/bin/activate (Linux/Mac)
venv\Scripts\activate (Windows)
pip install -r requirements.txt

Copy .env.example to .env and fill in your values (database URL, Twilio keys, secret key).

Initialize the database (if script provided):
python scripts/init_db.py

Run the server:
flask run

(Optional) Use ngrok to test Twilio webhooks:
ngrok http 5000

Project Structure
dryclean/
│-- app.py
│-- models.py
│-- views/
│-- webhooks/
│-- templates/
│-- static/
│-- scripts/
│-- requirements.txt
│-- README.md

Why This Project

Shows ability to design and implement a full product workflow

Demonstrates integration with third-party APIs (Twilio)

Includes clear documentation and setup steps recruiters can follow easily

Balances technical implementation with real business value

License-MIT
