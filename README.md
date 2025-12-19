# ShineOnYourDay 
# 🎉 Vow Venue - Marriage Hall Booking Platform

[![Project Banner](https://via.placeholder.com/1200x600.png?text=Vow+Venue+-+Marriage+Hall+Booking+Platform)](https://via.placeholder.com)

> A modern, responsive web application for browsing, booking, and managing marriage halls & banquet venues. Built with a focus on great user experience for customers and powerful admin controls.

## 🚀 Live Demo

- **Frontend Running at**: `http://localhost:5000` (after starting the dev server)
- **Fully functional demo** with simulated payments, pre-populated data, and role-based access

## 📸 Screenshots

*(Add actual screenshots later in /screenshots folder)*
- Home Page with featured venues
- Venue Detail & Gallery
- Multi-step Booking Wizard
- User Dashboard
- Admin Dashboard & Venue Management

## ✨ Key Features

- **User Authentication** (Register / Login / Role-based access)
- **Venue Browsing** with search, filters (price, capacity, amenities)
- **Advanced Booking System**
  - Interactive calendar with availability status (Green/Orange/Red)
  - Time slot selection: Morning, Evening, Full Day (different pricing)
  - Multi-step booking wizard with validation
- **Simulated Payment Gateway** (Stripe-like UI – use test card: 4242 4242 4242 4242)
- **User Dashboard** – View bookings, download PDF receipts
- **Powerful Admin Panel**
  - Statistics (total bookings, pending, revenue)
  - Booking verification & approval workflow
  - Full CRUD for venues
- **Responsive Design** – Works perfectly on mobile, tablet, and desktop
- **LocalStorage Persistence** – Data survives page refreshes

## 🧑‍💻 Test Accounts

### Admin (Full Access)
- Email: `admin@vow.com`
- Password: `admin`
- Redirects to: `/admin`

### Regular User (With existing bookings)
- Email: `rajesh@example.com`
- Password: `demo`
- Redirects to: `/dashboard`

## 🎭 Demo Guide & Testing Flow

### Quick Start
1. Run the project → Open `http://localhost:5000`
2. Browse featured venues on the homepage
3. Login with demo credentials or register a new account

### Recommended Demo Flow
1. Login as **rajesh@example.com** → Explore dashboard with pre-existing confirmed bookings
2. Browse venues → Filter → View details of "The Grand Crystal Ballroom"
3. Try booking a new date → Go through all 4 steps (Date → Details → Payment → Confirmation)
4. Logout → Login as **admin@vow.com**
5. Check admin dashboard → Verify pending bookings → Approve/Reject
6. Go to Venue Management → Add/Edit/Delete a venue

### Pre-loaded Demo Data
- 4 beautiful venues with images, descriptions, and amenities
- Multiple bookings (some confirmed, some pending verification)

## 🛠 Tech Stack

- **Frontend**: React.js + Vite
- **Backend** (Java Spring Boot)
- Java 17 or 21
- Spring Boot 3.x
- Spring Security + JWT
- Spring Data JPA (Hibernate)
- MySQL / PostgreSQL
- Lombok
- Validation (Bean Validation)
- Maven
- Optional: Spring Mail, PDF generation (iText), Stripe/Razorpay SDK
- **Styling**: Tailwind CSS + Custom Components
- **State Management**: React Context / useState
- **Routing**: React Router DOM
- **Form Handling**: React Hook Form
- **Calendar**: Custom built with date-fns
- **Data Storage**: Browser localStorage (for demo purposes)
- **Payment Simulation**: Custom form (no real transactions)
- **Icons**: Lucide React

## 📡 API Integration Ready

All API calls are centralized in `src/lib/api.ts`. Ready to connect to your backend (Java Spring Boot, Node.js, etc.):

```typescript
// Example endpoints
POST /api/auth/login
POST /api/auth/register
GET  /api/venues
GET  /api/venues/:id
POST /api/bookings
GET  /api/bookings/user/:userId
PATCH /api/admin/bookings/:id/status
// ...and more
