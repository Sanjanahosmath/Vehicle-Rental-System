# 🚗 Vehicle Rental System (C++ Console Application)

## 📌 Overview

The **Vehicle Rental System** is a C++ console-based application designed to simulate a real-world vehicle rental service. It provides role-based access for **admins** and **customers**, supports **vehicle renting and returning**, and uses **file storage** for persistent data handling.

---

## 📂 Features

### 👨‍💼 Admin Functionalities:
- 🔐 Admin login (default username: `admin`, password: `admin`)
- ➕ Add new vehicles (Car or Bike)
- 📄 View all vehicles
- 🧑‍💼 View customer database
- 💾 Save all data (vehicles and customers) to files

### 🧑‍💻 Customer Functionalities:
- 📝 Register as a new customer
- 🔐 Login using your name
- 🚘 View all available vehicles
- 🛵 Rent a vehicle
- 🔁 Return a rented vehicle
- 👤 View rental history and personal info

---

## 💾 File Storage

- `vehicles.txt` — stores all vehicle data with type and availability
- `customers.txt` — stores all customer info and rental records

All data is:
- ✅ Automatically loaded at program start
- 💾 Saved manually by the admin or on exit

---

## 🧱 System Design

### ✅ Object-Oriented Concepts Used:
- **Inheritance & Polymorphism** — `Vehicle` is a base class; `Car` and `Bike` inherit from it.
- **Encapsulation** — All related data and methods are encapsulated in relevant classes.
- **Dynamic Allocation** — Vehicles are stored using pointers and allocated dynamically.

### 🏗️ Classes and Their Roles

| Class       | Role / Responsibilities                                  |
|-------------|----------------------------------------------------------|
| `Vehicle`   | Base class for vehicle types                             |
| `Car`       | Derived from Vehicle, includes seat count                |
| `Bike`      | Derived from Vehicle, includes carrier flag              |
| `Customer`  | Stores customer data and their rental info               |
| `RentalShop`| Manages vehicles, customers, renting/returning, menus    |

---

## 🔁 Menu Flow

```text
Main Menu:
1. Admin
2. Register Customer
3. Customer Login
4. Exit

Admin Menu:
1. Add Vehicle
2. Show All Vehicles
3. Show All Customers
4. Save Data
5. Exit

Customer Menu:
1. View Vehicles
2. Rent Vehicle
3. Return Vehicle
4. View My Info
5. Exit
