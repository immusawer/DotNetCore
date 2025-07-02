# TestNetCore API

A simple .NET Core Web API project with CRUD operations for User and Product entities, using Entity Framework Core and SQL Server.

---

## 📋 Project Overview

- Built with **.NET Core 7** (or specify your version)
- Uses **Entity Framework Core** for ORM and migrations
- SQL Server database (local SQL Express instance)
- Swagger UI for API documentation and testing
- Supports full CRUD on Users and Products tables

---

## ⚙️ Prerequisites

Make sure you have these installed:

- [.NET SDK 7+](https://dotnet.microsoft.com/download)
- [SQL Server Express](https://aka.ms/ssms) with SQL Server Management Studio (optional but recommended)
- (Optional) [Git](https://git-scm.com/)

---

## 🔗 Database Connection String

Update your `appsettings.json` with the following connection string:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=localhost\\SQLEXPRESS;Database=TestDB;User Id=sa;Password=Musawer321;Encrypt=False;Trusted_Connection=False;MultipleActiveResultSets=true"
}
Note:

Encrypt=False disables SSL encryption for local development.

Ensure SQL Server allows SQL Authentication and sa login is enabled with the password above.

Alternatively, use Windows Authentication by changing Trusted_Connection=True and removing User Id and Password.

🚀 How to Run the Project Locally
Clone the repo

bash
Copy
Edit
git clone https://github.com/yourusername/TestNetCore.git
cd TestNetCore
Restore dependencies

bash
Copy
Edit
dotnet restore
Apply database migrations

bash
Copy
Edit
dotnet ef database update
Run the application

bash
Copy
Edit
dotnet run
The API will be running at http://localhost:5241

📖 API Documentation
Swagger UI is available for easy testing:

bash
Copy
Edit
http://localhost:5241/swagger
📦 Dependencies
The following NuGet packages are required and will be restored automatically on dotnet restore:

Microsoft.EntityFrameworkCore

Microsoft.EntityFrameworkCore.SqlServer

Microsoft.EntityFrameworkCore.Tools

Swashbuckle.AspNetCore (for Swagger UI)

If you need to install manually:

bash
Copy
Edit
dotnet add package Microsoft.EntityFrameworkCore
dotnet add package Microsoft.EntityFrameworkCore.SqlServer
dotnet add package Microsoft.EntityFrameworkCore.Tools
dotnet add package Swashbuckle.AspNetCore
⚡ Common Commands
Command	Description
dotnet restore	Restore NuGet packages
dotnet build	Build the project
dotnet ef migrations add NAME	Add a new EF migration
dotnet ef database update	Apply migrations to database
dotnet run	Run the application

🤝 Contributing
Feel free to fork and submit pull requests.
Open issues for bugs or feature requests.

📄 License
This project is licensed under the MIT License.

Made with ❤️ by Musawer Dinzad

yaml
Copy
Edit

---

If you want, I can help you create a `.gitignore` and give you instructions on how to push this project to GitHub!
```
