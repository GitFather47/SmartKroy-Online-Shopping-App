# SmartKroy Management System

SmartKroy is a modern Windows Forms (.NET 8, C# 12) application for managing products, categories, suppliers, and administrative records in a retail or inventory-based business. It features a user-friendly interface, robust CRUD operations, and SQL Server integration.

## Features

- **Admin Dashboard:** Central panel for managing products, categories, suppliers, and records.
- **Product Management:** Add, edit, delete, and view products with category assignment.
- **Category Management:** Manage product categories with descriptions and admin tracking.
- **Supplier Management:** Add, edit, and remove suppliers; supplier login and management.
- **User Management:** Create accounts, login, and manage customer information.
- **Record Keeping:** Maintain and view transaction or inventory records.
- **Modern UI:** Uses Guna UI2 controls for a visually appealing interface.
- **Database Integration:** Connects to SQL Server for persistent data storage.

## Technologies Used

- .NET 8 / C# 12
- Windows Forms (WinForms)
- Guna UI2 WinForms Controls
- Microsoft.Data.SqlClient (SQL Server)
- ADO.NET for database operations

## Getting Started

### Prerequisites

- Visual Studio 2022 or later
- .NET 8 SDK
- SQL Server (local or remote)
- Guna UI2 WinForms library (licensed)

### Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/GitFather47/SmartKroy-Online-Shopping-App
   ```

2. **Open the solution in Visual Studio.**

3. **Restore NuGet packages** if required.

4. **Configure the database connection string:**  
   Update the connection string in the code (e.g., `CatagoryForm.cs`) to match your SQL Server instance:
   ```
   Data Source=YOUR_SERVER; Initial Catalog=SmartKroy; Integrated Security=True; Trust Server Certificate=True
   ```

5. **Ensure the database schema exists:**  
   Create the required tables (`product_catagory`, `products`, `suppliers`, etc.) in your SQL Server database.

6. **Build and run the project.**

## Usage

- **Admin Login:** Use the admin login form to access the dashboard.
- **Navigation:** Use the sidebar to switch between Products, Categories, Suppliers, Records, and Admin Details.
- **CRUD Operations:** Use the provided forms to add, edit, or delete records.
- **Supplier Login:** Suppliers can log in and manage their information.

## Project Structure

- `AdminDashboard.cs` - Main admin panel and navigation
- `ManageProductsForm.cs` - Product management
- `CatagoryForm.cs` - Category management
- `ManageSuppliersForm.cs` - Supplier management
- `RecordForm.cs` - Record keeping
- `LoginForm.cs`, `AdminLogin.cs`, `Supplier_login.cs` - Authentication
- `HomeUser.cs`, `PCPartsUser.cs`, `HouseProductUser.cs`, `ClothesUser.cs` - User/customer modules

## Notes

- The UI uses Guna UI2 controls; ensure you have the library and a valid license.
- The application expects a pre-existing SQL Server database with the required tables.
- For demo/testing, you may need to adjust the connection string and seed the database with sample data.

## License

This project is for educational purposes. For commercial use, ensure compliance with third-party library licenses (e.g., Guna UI2).

---

*Developed with Visual Studio 2022 and .NET 8*
