# Minimal API (.NET 7) — Vehicle and Administrator Management

A lightweight **.NET 7 Minimal API** that demonstrates the use of JWT authentication, Entity Framework Core with MySQL, layered domain design, and Swagger documentation.

---

## 🚀 Features

- **JWT Authentication** with role-based authorization
- **Entity Framework Core** integration (MySQL provider)
- **Domain-driven structure** with DTOs, Services, and Interfaces
- **Swagger UI** for API exploration
- **CORS** support
- **Unit Tests** with sample services and mocks

---

## 🧩 Project Structure

```
minimal-api/
├── Api/
│ ├── Program.cs
│ ├── Startup.cs
│ ├── Dominio/
│ │ ├── DTOs/
│ │ ├── Entidades/
│ │ ├── Enuns/
│ │ ├── Interfaces/
│ │ ├── ModelViews/
│ │ └── Servicos/
│ ├── Infraestrutura/
│ │ └── DbContexto.cs
│ └── Migrations/
└── Test/
├── Domain/
├── Helpers/
├── Mocks/
└── Requests/
```


---

## ⚙️ Prerequisites

- [.NET 7 SDK](https://dotnet.microsoft.com/download/dotnet/7.0)
- [MySQL Server](https://www.mysql.com/)
- (Optional) [Visual Studio Code](https://code.visualstudio.com/) or Visual Studio 2022

---

## 🛠️ Setup & Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/danubiobwm/minimal-api-dio
   cd minimal-api-dio/Api

2. Configure Database
Edit appsettings.json and set your MySQL connection string under:
```
"ConnectionStrings": {
  "MySql": "server=localhost;database=MinimalApiDB;user=root;password=yourpassword"
},
"Jwt": {
  "Key": "your_secret_key"
}
```
3. Apply Migrations
```
dotnet ef database update
```
4. Run the API

```
dotnet run
```
5 . Open Swagger
```
Navigate to: http://localhost:5000/swagger
```

## 🔐 Authentication
Call /administradores/login with valid credentials:
```
{
  "email": "admin@example.com",
  "senha": "123456"
}
```
Copy the returned token and use it in the Authorization header:
```
Authorization: Bearer <your_token>
```

## 📚 API Endpoints

### Home
```
GET / → Returns API info
```
### Administradores
```
POST /administradores/login → Authenticate admin

GET /administradores → List all admins (Admin only)

POST /administradores → Create new admin (Admin only)
```
### Veiculos
```
GET /veiculos → List vehicles

POST /veiculos → Add new vehicle (Admin, Editor)

PUT /veiculos/{id} → Update vehicle (Admin only)

DELETE /veiculos/{id} → Delete vehicle (Admin only)
```

## 🧪 Testing
From the Test directory, run:
```
dotnet test
```

## 🧱 Technologies

.NET 7

Entity Framework Core

MySQL

JWT (System.IdentityModel.Tokens.Jwt)

Swagger / Swashbuckle

xUnit (for tests)

## 🧑‍💻 Author

Developed by Danubio
📧 danubio.bwm@gmail.com