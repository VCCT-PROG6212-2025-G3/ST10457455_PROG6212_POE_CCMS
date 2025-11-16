# 📘 Claim Capture Management System (CCMS)
### PROG6212 — Portfolio of Evidence (Part 3)  
**Student:** James Baker (ST10457455)

---

## 📑 Table of Contents
- [Project Overview](#-project-overview)
- [Features](#-features)
- [Technologies Used](#-technologies-used)
- [Project Structure](#-project-structure)
- [Database Design](#-database-design)
- [Screenshots Required](#-screenshots-required)
- [How to Run the Project](#️-how-to-run-the-project)
- [GitHub Version Control](#-github-version-control)
- [Presentation & Video Links](#-presentation--video-links)
- [Author](#-author)
- [Final Notes](#-final-notes)

---

## 📘 Project Overview

The Claim Capture Management System (CCMS) is an ASP.NET Core MVC web application created for PROG6212 POE Part 3.

It allows users to:
- Capture contractor information  
- Manage contracts  
- Record monthly claims  
- Automatically calculate totals  
- View a consolidated summary  

The system uses EF Core with SQLite, MVC architecture, and clean UI design.

---

## ⭐ Features

### 🔹 Contractor Management
- Create, edit, delete contractors  
- View list of all contractors  

### 🔹 Contract Management
- Assign contracts to contractors  
- Set hourly rate  
- Edit and delete contracts  

### 🔹 Monthly Claims
- Capture hours  
- System automatically calculates claim total  
- Connected to contract rate  

### 🔹 Summary Report
- LINQ join across all tables  
- Contractor → Contract → Claim details  
- Displays totals clearly  

### 🔹 Additional Features
- MVC architecture  
- Bootstrap UI  
- Error handling  
- SQLite integration  
- EF Core migrations  

---

## 🛠 Technologies Used

- ASP.NET Core 8 MVC  
- C#  
- Entity Framework Core  
- SQLite  
- Razor Views  
- Bootstrap 5  
- LINQ  
- Git & GitHub  

---

## 📁 Project Structure

📂 ClaimSystem.Web
┣ 📁 Controllers
┣ 📁 Models
┣ 📁 Views
┣ 📁 Data
┣ 📁 Migrations
┣ 📁 wwwroot
┣ Program.cs
┣ appsettings.json
┗ ClaimSystem.Web.csproj

yaml
Copy code

---

## 🗄 Database Design

### 📌 Entities

#### 1️⃣ Contractor
- ContractorId  
- FirstName  
- LastName  
- Email  

#### 2️⃣ Contract
- ContractId  
- ContractorId  
- Description  
- Rate  

#### 3️⃣ MonthlyClaim
- ClaimId  
- ContractId  
- Hours  
- Total  

---

### 🔗 Relationships
- One Contractor → Many Contracts  
- One Contract → Many MonthlyClaims  

---

### 🧮 Claim Calculation Formula

Total = Hours × Rate

yaml
Copy code

---

## 📸 Screenshots Required

### 1️⃣ EF Core Registration (Program.cs)
*Insert screenshot here*  
**Caption:** Figure 1 – EF Core and SQLite configuration.

---

### 2️⃣ SQLite Database Diagram
*Insert screenshot here*  
**Caption:** Figure 2 – Database tables (Contractors, Contracts, MonthlyClaims).

---

### 3️⃣ Contractor CRUD Pages
*Insert screenshots*  
**Caption:** Figure 3 – Contractor management (List, Create, Edit).

---

### 4️⃣ Contract CRUD Pages
*Insert screenshots*  
**Caption:** Figure 4 – Contract management pages.

---

### 5️⃣ Monthly Claims Pages
*Insert screenshots*  
**Caption:** Figure 5 – Monthly claims with automatic totals.

---

### 6️⃣ Summary Page
*Insert screenshot*  
**Caption:** Figure 6 – Summary LINQ view.

---

## ▶️ How to Run the Project

### 1️⃣ Restore Dependencies
dotnet restore

shell
Copy code

### 2️⃣ Apply Migrations
dotnet ef database update

shell
Copy code

### 3️⃣ Run the System
dotnet run

yaml
Copy code

The website will launch at:  
- http://localhost:5000  
- https://localhost:7000  

---

## 🔀 GitHub Version Control

This project includes:
- Proper commit structure  
- Clean remote origin setup  
- No nested repos  
- Full project source included  

---

## 🎤 Presentation & Video Links

### 🎞 YouTube Demonstration
👉 *Paste your YouTube link here*

### 🖥 PowerPoint Presentation
👉 *Paste your PowerPoint (.pptx) link here*

---

## 👨‍💻 Author

**James Baker**  
**Student Number:** ST10457455  
PROG6212 — Portfolio of Evidence (Part 3)

---

## ⭐ Final Notes

This project demonstrates:
- Strong ASP.NET Core MVC development  
- Data modelling and EF Core migrations  
- Complete CRUD functionality  
- Good UI structure  
- Professional Git usage  
- Practical LINQ reporting  

✔ Fully functional  
✔ Clean architecture  
✔ Meets POE requirements  

---
