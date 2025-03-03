# 🚍 GoPass Project

## 📌 Overview
The **GoPass Project** is an enhancement to the existing GoPass transit application, aiming to improve public transportation usability by introducing:
- **Seat Reservations** 🪑: Users can pre-book a seat on the bus.
- **Live Bus Tracking** 📍: Real-time GPS tracking for better commute planning.
- **Promo Code System** 🎟️: Discounts based on travel history.

## 🏆 Key Features
- **Reserve a Seat**: Users can check bus availability and reserve seats before arrival.
- **Live Tracking**: Real-time GPS tracking via QR-based driver check-ins.
- **Bus Schedule Lookup**: Fetch route details and estimated arrival times.
- **Promo Codes & Discounts**: Riders can redeem points for travel discounts.
- **Database-Backed System**: Secure and efficient data handling for transactions and schedules.

---

## 🔧 Technology Stack
| Component        | Technology Used |
|-----------------|----------------|
| **Frontend**    | React, HTML, CSS |
| **Backend**     | Python (Flask/Django) |
| **Database**    | PostgreSQL / MySQL |
| **Cloud Services** | AWS (EC2, RDS, Lambda) |
| **APIs**        | Google Maps API, DART API |
| **Version Control** | Git & GitHub |

---

## 🖥️ System Architecture
The project consists of:
1. **Frontend**: User interface for booking, payments, and tracking.
2. **Backend API**: Manages user requests, authentication, and data processing.
3. **Database**: Stores bus schedules, reservations, and user transactions.
4. **Live Tracking Module**: Uses GPS and QR scans to update bus locations.

---

## 📌 Features Breakdown
### 🪑 **Reserve A Seat**
- Users can search for available buses along their route.
- Seat availability is displayed in real-time.
- Payment processing ensures seat reservation.

### 📍 **Live Bus Tracking**
- Drivers check in using QR codes.
- GPS tracking updates every few seconds.
- Users can track buses and estimated arrival times.

### ⏳ **Get Bus Schedule**
- Users can look up bus stops and schedules.
- Estimated time of arrival (ETA) is dynamically calculated.

### 🎟️ **Apply Promo Code**
- Users earn points for trips.
- Points can be redeemed for discount codes.

---

## 🏗️ Installation & Setup
### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/gopass-project.git
cd gopass-project


### 2️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 3️⃣ Setup Database
```bash
python manage.py migrate
```

### 4️⃣ Run the Server
```bash
python manage.py runserver
```
🚀 Now, the application should be running at `http://localhost:8000/`

---

## 📊 Database Schema
| Table Name   | Fields |
|-------------|-----------------------------------------------------------|
| **Users** | `id, name, email, password, points` |
| **Buses** | `bus_id, route, capacity, available_seats` |
| **Reservations** | `reservation_id, user_id, bus_id, seat_number, payment_status` |
| **Driver Check-in** | `driver_id, bus_id, gps_location, timestamp` |
| **Promo Codes** | `promo_id, discount, expiry_date` |

---

## 📜 API Endpoints
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/reserve-seat` | `POST` | Reserve a seat for a specific bus |
| `/api/get-bus-schedule` | `GET` | Retrieve schedule for a bus stop |
| `/api/live-tracking` | `GET` | Fetch live GPS location of a bus |
| `/api/apply-promo` | `POST` | Apply promo code for discounts |

---

## 📌 Future Enhancements
✅ **AI-based Demand Prediction** for better seat allocation  
✅ **Voice Assistant Integration** for hands-free booking  
✅ **Multi-language Support** for diverse users  

---

## 👨‍💻 Contributors
- **Nikhil Sai Vemula** (Backend & Database)
- **Monika Vaddineni** (UI/UX & API Integration)
- **Sriya Namavarapu** (Project Documentation & Testing)

---

## 🎯 License
This project is licensed under the **MIT License**.

---

🚀 **Start using GoPass today and never miss a seat!**
```

This **README.md** is well-structured for GitHub and includes:
- Project Overview
- Features
- Tech Stack
- System Architecture
- Setup Instructions
- Database Schema
- API Endpoints
- Future Enhancements
- Contributors

Let me know if you need any modifications! 🚀
