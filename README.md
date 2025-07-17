# Internal Resource Booking System

This is a web application built with **ASP.NET Core MVC**, **Entity Framework Core**, and **MySQL/SQL Server**. It allows users to manage resources and create bookings with proper conflict detection and validation.

---

## 🛠 Features

- Full **CRUD** operations for:
  - Resources (e.g., rooms, equipment)
  - Bookings (with date/time conflict validation)
- Server-side and client-side **form validation**
- Responsive UI using **Bootstrap**
- Clean, maintainable **C# code**
- Uses **EF Core** with **MySQL** (via Pomelo) or **SQL Server**
- Razor Views for dynamic rendering

---

## 📁 Project Structure

BookingWeb/
├── Controllers/
├── Models/
├── Views/
├── Data/ (ApplicationDbContext)
├── wwwroot/
├── appsettings.json
└── Program.cs
