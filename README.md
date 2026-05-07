# ✈️ Airline Reservation & Booking System

A modern **Airline Reservation and Booking System** built using **Django**, featuring flight booking, passenger management, payment integration, admin panel, authentication system, and responsive UI.

---

# 🚀 Features

## 👤 User Features

* User Registration & Login
* Flight Search & Booking
* Passenger Management
* Destination & Travel Experience Pages
* Loyalty Program Information
* Payment Gateway Integration
* Booking Confirmation

---

## 🛠️ Admin Features

* Admin Dashboard
* Manage Flights
* Manage Passengers
* View Bookings
* Manage Payments

---

# 🧰 Technologies Used

* Python
* Django
* SQLite3
* HTML5
* CSS3
* JavaScript
* Streamlit
* Bootstrap
* Vercel Deployment

---

# 📁 Project Structure

```text
airline_system/
│
├── admin_panel/
├── airline_system/
├── payment/
├── static/
│   └── css/
│       └── styles.css
│
├── templates/
│   ├── home.html
│   ├── login.html
│   ├── register.html
│   ├── book.html
│   ├── results.html
│   ├── passengers.html
│   ├── manage.html
│   ├── Destination.html
│   ├── Experience.html
│   ├── Help.html
│   ├── Loyality.html
│   └── spline.html
│
├── db.sqlite3
├── manage.py
├── requirements.txt
├── vercel.js
└── README.md
```

---

# ⚙️ Installation & Setup

## 🔷 1. Clone Repository

```bash
git clone <your-repository-url>
```

---

## 🔷 2. Navigate to Project Folder

```bash
cd airline_system
```

---

## 🔷 3. Create Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

---

## 🔷 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

# 🗄️ Database Setup

## Apply Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

---

# 👤 Create Superuser (Admin)

```bash
python manage.py createsuperuser
```

Enter:

* Username
* Email
* Password

---

# ▶️ Run Development Server

```bash
python manage.py runserver
```

---

# 🌐 Open in Browser

```text
http://127.0.0.1:8000
```

---

# 🔐 Admin Panel

```text
http://127.0.0.1:8000/admin
```

Login using superuser credentials.

---

# 💳 Payment Module

Payment pages available:

* payment_page.html
* success.html

Features:

* Payment processing simulation
* Booking success confirmation

---

# 📸 Main Pages

* 🏠 Home Page
* ✈️ Flight Booking
* 👥 Passenger Details
* 📍 Destinations
* 🌟 Travel Experience
* 💎 Loyalty Program
* ❓ Help & Support

---

# 🎨 UI Features

* Responsive Design
* Modern Airline Theme
* Interactive Pages
* Smooth Navigation
* Clean CSS Styling

---

# ☁️ Deployment

This project includes:

* `vercel.js` configuration
* Ready for Vercel deployment

---

# 📦 requirements.txt Installation

Example dependencies:

```text
Django
streamlit
gunicorn
```

Install all:

```bash
pip install -r requirements.txt
```

---

# 🧪 Run Streamlit App (Optional)

```bash
streamlit run streamlit_app.py
```

---

# 🚀 Future Enhancements

* Online Payment Gateway Integration
* Real-time Flight Tracking
* Seat Selection System
* Email Notifications
* AI-based Flight Recommendations

---

# 👨‍💻 Author

**Shreyas Narsale**

GitHub:
[shreyasnarsale](https://github.com/shreyasnarsale?utm_source=chatgpt.com)

---

# 📄 License

This project is for educational and learning purposes.

Licensed under the MIT License.

---

# ⭐ Support

If you like this project:

* Star the repository ⭐
* Fork the project 🍴
* Share with others 🚀

---

# ✈️ Happy Coding & Safe Travels!
