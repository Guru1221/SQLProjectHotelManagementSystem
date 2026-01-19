# SQLProjectHotelManagementSystem

## 📌 Project Overview
This project is a **comprehensive SQL-based Hotel Management System** designed to manage hotel operations, including customer bookings, room inventory, staff management, and payment processing. 

Unlike basic databases, this project implements **advanced database automation** using **Triggers** to ensure data consistency and **Views** for simplified reporting.

## 🛠️ Tech Stack
- **Database:** MySQL
- **Language:** SQL (DDL, DML, DQL, TCL)
- **Advanced Features:** Triggers, Views, Stored Procedures

## 📂 Database Schema
The system is built on a normalized relational schema with 5 core tables:

1. **Customers**: Stores guest details (Name, Email, Phone, Location).
2. **Rooms**: Inventory of rooms with types (e.g., Suite, Deluxe), capacity, and pricing.
3. **Staff**: Employee records including roles and contact info.
4. **Bookings**: The central transactional table linking Customers, Rooms, and Staff with check-in/out dates.
5. **Payments**: Records financial transactions linked to specific bookings.

## 🚀 Key Features & Scenarios Handled
This project solves complex business logic problems using advanced SQL concepts:

### 1. Database Automation (Triggers)
- **Data Integrity**: Prevents logical errors, such as ensuring a guest cannot check out before they check in (`ValidateBookingDates`).
- **Cascading Deletes**: Automatically removes payment records if a booking is cancelled (`DeletePaymentWHENBookingDelete`).
- **Auto-Updates**: Automatically updates booking totals when new payments are recorded.

### 2. Reporting (Views)
- **High-Value Customer Tracking**: A dedicated View (`HighValueBookings`) instantly retrieves all bookings exceeding ₹20,000, simplifying revenue analysis.

### 3. Data Analysis
- **String Manipulation**: Formats output for reports (e.g., combining ID, Method, and Amount into a single readable string).
- **Transactional Queries**: Handles complex limits and ordering to find recent payments.

## 💻 How to Use
1. **Clone the Repository**:
   ```bash
   git clone [https://github.com/your-username/Hotel-Management-SQL.git](https://github.com/your-username/Hotel-Management-SQL.git)
