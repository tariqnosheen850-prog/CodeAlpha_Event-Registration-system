# CodeAlpha Event Registration System

A complete backend **Event Registration System** built with **Django** and **Django REST Framework** as part of CodeAlpha Internship Task.

## Features
- View list of events
- View detailed information of a specific event
- Register for events
- View your own registrations
- Cancel registrations
- Token-based authentication
- Full Admin Panel for event organizers
- Capacity management & registration deadlines

## Tech Stack
- **Backend**: Django + Django REST Framework
- **Database**: SQLite (can be easily switched to PostgreSQL)
- **Authentication**: Token Authentication
- **Extra**: Django Admin Panel, CORS support

## Installation & Setup

```bash
# Clone the repository
git clone https://github.com/tariqnosheen850-prog/CodeAlpha_Event-Registration-system.git
cd CodeAlpha_Event-Registration-system

# Create virtual environment
python -m venv venv
venv\Scripts\activate          # Windows
# source venv/bin/activate     # Mac/Linux

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Create superuser (for admin panel)
python manage.py createsuperuser

# Start the server
python manage.py runserver
## API Endpoints

| Method | Endpoint                    | Description                        |
|--------|-----------------------------|------------------------------------|
| GET    | `/api/events/`              | List all events                    |
| GET    | `/api/events/<id>/`         | Get event details                  |
| POST   | `/api/events/`              | Create new event (Admin)           |
| POST   | `/api/register/`            | Register for an event              |
| GET    | `/api/registrations/`       | View your registrations            |
| DELETE | `/api/registrations/<id>/`  | Cancel registration                |
| POST   | `/api/token/`               | Get authentication token           |
## How to Test
- Start the server → `http://127.0.0.1:8000/`
- Admin panel: `http://127.0.0.1:8000/admin/`
- You can test the APIs using Postman

## Author
**Tariq Nosheen**  
CodeAlpha Intern
