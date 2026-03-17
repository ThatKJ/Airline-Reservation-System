# ✈️ Airline Reservation System (Python + MySQL)

A terminal-based Airline Reservation System built in Python using MySQL for persistent storage. The system supports both users and admins, allowing flight booking, seat selection, cancellations, reporting, and more!

---

## 📁 Project Structure
```
📁 Project Root
├── main.py 
├── db_setup.sql 
├── requirements.txt 
├── README.md
└── 📁 app/
├── 📁 auth/ # Login/Signup system
├── 📁 admin/ # Admin-only features
├── 📁 user/ # Booking, seat selection, search, etc.
└── db.py # MySQL database connector
```
## 🚀 Features

### 👤 User Features:
- Sign up & Login
- Book flight with seat selection
- Cancel booking
- View all available flights
- Search flights by source, destination, and date
- View booking history

### 🛫 Admin Features:
- Admin login/signup
- Add or delete flights
- Manage flight status (Scheduled, Delayed, Cancelled)
- View dashboard: total users, bookings, revenue
- Generate reports
- Export all reservations to CSV

## 🛠️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/ThatKJ/airline-reservation-system.git
cd airline-reservation-system

2. Install dependencies
pip install -r requirements.txt

3. Set up MySQL database
Open MySQL and run the SQL script:
```
```bash
source db_setup.sql;
```
This creates the database airline_db with all required tables.

4. Configure DB Connection
Make sure the app/db.py has your correct DB credentials:
```
mysql.connector.connect(
    host="localhost",
    user="root",
    password="your_mysql_password",
    database="airline_db"
)
```

✅ How to Run
From your project directory:

python main.py

🤝 Contributing
Contributions are welcome! If you'd like to add a feature or fix a bug, feel free to open a pull request.

📄 License
MIT License – Use it freely and make something cool 🚀
