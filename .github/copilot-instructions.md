# AI Assistant Instructions - Airline Reservation System

## Project Overview
Django-based airline reservation system using MongoDB for data storage. Key components:
- Frontend: Django templates in `/templates` and app-specific template directories
- Backend: Django apps (`admin_panel`, `payment`, `airline_system`) with direct MongoDB access
- Integrations: Razorpay payments, MongoDB Atlas, SMTP for emails

## Essential Patterns

### MongoDB Usage
```python
# Always use direct pymongo queries (not Django ORM)
from pymongo import MongoClient
db = client['airline_reservation_system']

# Query pattern: list + ID string conversion
items = list(db.flights.find({'departure_city': city}))
for item in items:
    item['id'] = str(item['_id'])  # Convert ObjectId for templates
```

### View & Template Conventions
- Convert MongoDB `ObjectId` to string before template context
- Wrap form/URL IDs with `ObjectId()` in view handlers
- Template context keys: `items`, `flights`, `employees`, etc.
- Access converted IDs in templates as `.id` (not `._id`)

### Authentication Flow
Custom cookie/session-based auth without Django User model:
```python
user_id = request.COOKIES.get('user_id')
if user_id:
    user = users.find_one({"_id": ObjectId(user_id)})
    if user:
        # User is authenticated
```

## Quick Reference
- **Date handling**: Use `datetime.strptime(str_date, "%Y-%m-%dT%H:%M")` for forms
- **DB collections**: flights, users, bookings, payments, special_services
- **Key URLs**: home/, admin/, payment/
- **Auth roles**: Admin vs Employee (check `role` field in users collection)

## Development Setup
```bash
python -m venv .venv
.venv\Scripts\Activate.ps1  # Windows
pip install -r requirements.txt
python manage.py runserver
```

## Security Notes
- MongoDB connection strings in `views.py` - use env vars in production
- Razorpay/SMTP credentials in `settings.py` - use env vars in production