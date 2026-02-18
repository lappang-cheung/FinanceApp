# 💰 FinanceApp -- Simple ASP.NET Core MVC Learning Project

## 📌 Overview

FinanceApp is a simple ASP.NET Core MVC application built to learn:

-   ASP.NET Core MVC architecture
-   Entity Framework Core
-   SQL Server / LocalDB integration
-   CRUD operations
-   Dependency Injection
-   Service layer pattern

This project allows users to create and view expenses while
understanding how data flows from the controller to the database.

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   ASP.NET Core MVC
-   Entity Framework Core
-   SQL Server (LocalDB)
-   C#
-   Razor Views

------------------------------------------------------------------------
## 📂 Project Structure

```
FinanceApp
│
├── Controllers
│   └── ExpensesController.cs
│
├── Models
│   └── Expense.cs
│
├── Data
│   ├── FinanceAppContext.cs
│   └── Service
│       ├── iExpensesService.cs
│       └── ExpensesService.cs
│
├── Views
│   └── Expenses
│       ├── Index.cshtml
│       └── Create.cshtml
│
├── appsettings.json
└── Program.cs
```


------------------------------------------------------------------------

## 🧠 Features

-   View all expenses
-   Add a new expense
-   Server-side validation using Data Annotations
-   Database persistence with EF Core
-   Separation of concerns using a service layer

------------------------------------------------------------------------

## 🗄️ Database Setup

This app uses SQL Server LocalDB.

### 1️⃣ Configure Connection String

In appsettings.json:

{ "ConnectionStrings": { "DefaultConnection":
"Server=(localdb)\\mssqllocaldb;Database=FinanceAppDb;Trusted_Connection=True;MultipleActiveResultSets=true"
} }

------------------------------------------------------------------------

### 2️⃣ Run Migrations

Open Package Manager Console and run:

Add-Migration InitialCreate Update-Database

This will create the database and the Expenses table.

------------------------------------------------------------------------

## 🚀 Running the Application

1.  Clone the repository
2.  Restore NuGet packages
3.  Run migrations
4.  Press F5 or run:

dotnet run

5.  Navigate to:

/Expenses

------------------------------------------------------------------------

## 📖 What I Learned

-   How the MVC pattern works in ASP.NET Core
-   How Dependency Injection is configured and used
-   How to configure and register a DbContext
-   How EF Core handles database operations
-   How to implement a service layer for better architecture

------------------------------------------------------------------------

## 🔮 Future Improvements

-   Edit and Delete functionality
-   Expense categories and filtering
-   Dashboard with charts
-   Authentication and user accounts
-   REST API version

------------------------------------------------------------------------

## 🎯 Purpose

This project was built as a learning exercise to understand the
fundamentals of ASP.NET Core MVC and Entity Framework Core before
building larger, production-level applications.
