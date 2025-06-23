📚 BookSpace  
BookSpace is a .NET Core web application designed to manage books, categories, and related data using a clean architecture approach. It supports Entity Framework Core for database operations and is built with scalability and maintainability in mind.

🚀 Features  
🔸 Book and category management  
🔸 SQL Server / Azure SQL Edge support  
🔸 Entity Framework Core integration  
🔸 Layered architecture (API, Application, Infrastructure, Domain)  
🔸 RESTful API endpoints  
🔸 Docker-compatible SQL support  

🏗️ Project Structure  
BookSpace/  
├── API           # ASP.NET Core Web API (entry point)  
├── Infrastructure # Data access layer (EF Core)  
├── Core           # Domain models and interfaces  
├── BookSpace.sln            # Solution file  

🔧 Technologies Used  
.NET 8 (ASP.NET Core)  
Entity Framework Core  
SQL Server / Azure SQL Edge  
Docker (optional)  
C#  
RESTful APIs  

🐳 Run with Docker (SQL Edge)  
To run SQL Server using Docker:

```bash
docker run -e "ACCEPT_EULA=Y" -e "SA_PASSWORD=YourStrong!Passw0rd" -p 1434:1433 --name bookspace-sql -d mcr.microsoft.com/azure-sql-edge
