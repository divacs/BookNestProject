# BookNestProject# 📚 BookNest  

**BookNest** is a modern web application built with **.NET 8**, designed for **buying, ordering, and managing books**.  
In addition to e-commerce features, the application also includes a **project management system** where admins can manage users, orders, and content.  

---

## 🚀 Technologies & Architecture  

- **.NET 8 MVC** with Razor Pages  
- **N-Tier Architecture** (Presentation, Application, Infrastructure, Domain)  
- **Repository Pattern + Unit of Work**  
- **Entity Framework Core** (Code First + Migrations)  
- **Scaffold Identity (Razor Class Library)**  
- **Roles & Authorization (Admin, Manager, Customer)**  
- **ViewData / ViewBag / TempData** for data passing  
- **Session Management** in .NET Core  
- **View Components** for reusability  

---

## 🎯 Features  

- ✅ Book purchase and ordering  
- ✅ User management (admin panel)  
- ✅ Project Management system (admin privileges)  
- ✅ Stripe integration (payment and refund)  
- ✅ Social login (Facebook)  
- ✅ Email notifications (SendGrid)  
- ✅ Rich Text Editor for content input  
- ✅ SweetAlert integration for UX  
- ✅ DataTables for listing and searching  
- ✅ Database seeding with `DbInitializer`  
- ✅ Deploy to Azure  

---

## 🏗️ Project Architecture  

```
BookNest/
│-- BookNest.Web (UI Layer - MVC + Razor Pages + API Controllers)
│-- BookNest.Application (Business logic, DTOs, Services)
│-- BookNest.Infrastructure (EF Core, Repositories, UnitOfWork, DbInitializer)
│-- BookNest.Domain (Entities, Models)
│-- BookNest.Tests (Unit & Integration Tests)
```

---

## ⚡ Installation & Setup  

1. Clone the repo  
```bash
git clone https://github.com/username/BookNest.git
cd BookNest
```

2. Create the database and apply migrations  
```bash
dotnet ef database update
```

3. Run the application  
```bash
dotnet run --project BookNest.Web
```

4. Open in browser  
```
https://localhost:5001
```

---

## 🔑 Roles & Login  

- **Admin** – full access (manage books, users, orders)  
- **Manager** – order and reporting access  
- **Customer** – purchase and order tracking  

👉 Admin is automatically created via `DbInitializer` (default credentials: `admin@booknest.com / Admin123*`).  

---

## ☁️ Deployment  

The application is ready for **Azure App Service** deployment.  
Supports:  
- Azure SQL connection string  
- SendGrid API Key  
- Stripe API Key  
- Facebook App ID/Secret  

---

## 📬 Contact  

👩‍💻 Author: Sonja Divac 
📧 Email: sonja.divac@yahoo.com  

---

✨ **BookNest** is built as a showcase project for modern .NET 8 practices and real-world e-commerce applications.  
