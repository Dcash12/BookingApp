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

```
BookingWeb/
├── Controllers/
├── Models/
├── Views/
├── Data/ (ApplicationDbContext)
├── wwwroot/
├── appsettings.json
└── Program.cs
```

---

## 🔧 Prerequisites

- [.NET SDK 7.0+](https://dotnet.microsoft.com/download)
- [Visual Studio 2022](https://visualstudio.microsoft.com/) or [VS Code](https://code.visualstudio.com/)
- MySQL or SQL Server
- (Optional) Git for version control

---

## 🔌 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/resource-booking-system.git
cd resource-booking-system
```

### 2. Configure Database Connection

In `appsettings.json`, set your DB connection string:

```json
"ConnectionStrings": {
  "Default": "server=localhost;database=BookingDb;user=root;password=yourpassword;"
}
```

For SQL Server:
```json
"Default": "Server=(localdb)\\MSSQLLocalDB;Database=BookingDb;Trusted_Connection=True;"
```

### 3. Run Migrations & Update Database

```bash
dotnet ef migrations add InitialCreate
dotnet ef database update
```

### 4. Run the App

```bash
dotnet run
```

Visit `https://localhost:5001` in your browser.

---

## ✅ Usage

- Navigate to `/Resources` to manage available resources.
- Navigate to `/Bookings` to create, view, or cancel bookings.
- Booking form ensures no overlapping bookings are allowed.

---

## 📌 Important Notes

- Booking conflict logic is implemented in `BookingController`.
- Uses Pomelo.EntityFrameworkCore.MySql for MySQL compatibility.
- Server-side validation via data annotations (e.g., `[Required]`, `[DataType]`, etc.)

---

## 🧑‍💻 Developer Info

**Name**: Kealeboga Saku  
**Role**: Junior ASP.NET Core Developer   
**Email**: Kealebogasaku2@gmail.com

---

## 📜 License

This project is for technical assessment and educational purposes.
