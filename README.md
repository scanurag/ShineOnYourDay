# 🌟 ShineOnYourDay  
## 🎉 Vow Venue – Marriage Hall Booking Platform

![Project Banner](https://github.com/scanurag/ShineOnYourDay/blob/f42fc3a7abd90390455756da12ef6417206505cd/Screenshot%202025-12-12%20215247.png)

> A modern, responsive web application for browsing, booking, and managing marriage halls & banquet venues.  
> Designed with a seamless user experience and powerful admin controls.

---

## 🚀 Live Demo

- **Frontend URL**: `http://localhost:5000` (after starting dev server)
- Fully functional demo with:
  - Simulated payments
  - Preloaded venues & bookings
  - Role-based authentication

---

## 📸 Application Screenshots

### 🏠 Home & Venue Browsing
![Home](https://github.com/scanurag/ShineOnYourDay/blob/e3d31f6883593999cd07b219fd258f4bbe52d9b4/Screenshot%202025-12-12%20215304.png)
![Booking Step](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215415.png)
![Venue Details](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215338.png)

### 📅 Booking Flow
![Calendar](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215359.png)
![Booking Step](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215415.png)
![Payment](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215533.png)
![Confirmation](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215558.png)

### 👤 User Dashboard
![User Dashboard](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215610.png)
![Bookings](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215706.png)

### 🛠 Admin Panel
![Admin Dashboard](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-12%20215720.png)
![Admin Stats](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-22%20143313.png)
![Venue Management](https://github.com/scanurag/ShineOnYourDay/blob/0fb30ea4775c26b4022c9624dfe1910fc75ab64e/Screenshot%202025-12-22%20143421.png)

---

## ✨ Key Features

### 👥 User Features
- User authentication (Register / Login)
- Browse venues with filters (price, capacity, amenities)
- Venue gallery & detailed info
- Multi-step booking wizard
- Interactive availability calendar (Green / Orange / Red)
- Time slots:
  - Morning
  - Evening
  - Full Day
- Simulated payment gateway
- Downloadable PDF receipts
- User dashboard with booking history

### 🧑‍💼 Admin Features
- Admin dashboard with analytics
- Booking approval / rejection
- Revenue & booking statistics
- Full CRUD for venues
- Role-based access control

---

## 🧪 Test Accounts

### 🔐 Admin
- **Email**: `admin@vow.com`
- **Password**: `admin`
- **Route**: `/admin`

### 👤 User
- **Email**: `rajesh@example.com`
- **Password**: `demo`
- **Route**: `/dashboard`

---

## 🎭 Demo Walkthrough

1. Login as **rajesh@example.com**
2. Browse venues → Book a new date
3. Complete booking wizard
4. Make payment using test card  
   `4242 4242 4242 4242`
5. Logout → Login as **admin**
6. Approve or reject pending bookings
7. Manage venues

---

## 🛠 Tech Stack

### Frontend
- React.js + Vite
- Tailwind CSS
- React Router DOM
- React Hook Form
- Context API
- Lucide Icons
- date-fns

### Backend (Pluggable)
- Java 17 / 21
- Spring Boot 3.x
- Spring Security + JWT
- Hibernate (JPA)
- MySQL / PostgreSQL
- Maven
- Lombok

### Other
- LocalStorage (Demo persistence)
- Simulated payment gateway
- PDF generation ready
- API-ready architecture

---

## 📡 API Endpoints (Ready)

```ts
POST   /api/auth/login
POST   /api/auth/register
GET    /api/venues
GET    /api/venues/:id
POST   /api/bookings
GET    /api/bookings/user/:userId
PATCH  /api/admin/bookings/:id/status

