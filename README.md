# E-commerce Web Application

A full-featured e-commerce web application built with ASP.NET Core 8.0 and Entity Framework Core using SQLite database.

## Features

- User Authentication and Authorization
  - Identity-based authentication
  - Role-based authorization (Admin/User roles)
  - User profile management
  - Password recovery
  - Email confirmation
  
- Admin Area
  - Product management (CRUD operations)
  - Category management
  - Product type management
  - User management
  - Role management

- Customer Area
  - Product browsing
  - Shopping cart
  - Order management
  - Product comments/reviews
  - User profile settings

## Technologies

- ASP.NET Core 8.0
- Entity Framework Core
- SQLite Database
- ASP.NET Core Identity
- Bootstrap
- Razor Pages
- MVC Architecture

## Prerequisites

- .NET SDK 8.0 or later
- Visual Studio 2022 or Visual Studio Code

## Getting Started

1. Clone the repository
```sh
git clone <repository-url>
```
2. Navigate to the project directory
```
cd EcommerceWeb
```
3. Restore dependencies
```
dotnet restore
```
4. Run database migrations
```
dotnet ef database update
```
5. Run the application
```
dotnet run
```

The application will automatically create an admin role and admin user on first run.

## Project Structure
- `Areas/`: Contains feature-specific areas
    - `Admin/`: Administrative features
    - `Customer/`: Customer-facing features
    - `Identity/`: Authentication and user management
- `Data/`: Database context and migrations
- `Models/`: Application domain models
- `Views/`: MVC views and Razor Pages
- `wwwroot/`: Static files (CSS, JavaScript, images)

## Database Schema
The application uses Entity Framework Core with SQLite and includes the following main entities:

- ApplicationUser
- Products
- Categories
- ProductTypes
- Orders
- OrderDetails
- Comments