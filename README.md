# IndieGameZone.Backend

![.NET 8](https://img.shields.io/badge/.NET-8-512BD4?logo=dotnet)
![.NET Aspire](https://img.shields.io/badge/.NET_Aspire-✓-512BD4?logo=dotnet)
![Docker](https://img.shields.io/badge/Docker-✓-2496ED?logo=docker)
![EF Core](https://img.shields.io/badge/EF_Core-✓-512BD4)
![JWT](https://img.shields.io/badge/JWT-Auth-yellow)
![License](https://img.shields.io/badge/License-MIT-green)

A modern, scalable backend API for indie game distribution platforms (inspired by itch.io), built with **.NET 8** and **.NET Aspire**.

## 🚀 Features

- **Clean Architecture** with separated layers:
  - `BusinessObject` (Domain models)
  - `Repository` (Repositories, DbContext)
  - `Service` (Business logic)
  - `API` (REST endpoints)
- **.NET Aspire** for cloud-native orchestration
- **Docker** container support
- Repository Pattern + Unit of Work
- JWT Authentication (planned)

## 📂 Solution Structure

IndieGameZone.Backend/ <br>
├── IndieGameZone.API/ # Web API (Entry Point) <br>
├── IndieGameZone.BusinessObject/ # Domain Models/Entities <br>
├── IndieGameZone.Repository/ # Data Access (EF Core) <br>
├── IndieGameZone.Service/ # Business Logic <br>
└── IndieGameZone.AppHost/ # .NET Aspire Orchestration <br>

## 🛠️ Prerequisites

- [.NET 8 SDK](https://dotnet.microsoft.com/download)
- [Docker Desktop](https://www.docker.com/products/docker-desktop) (optional)
- IDE (VS 2022+, VS Code, or Rider)

## 🏃 Getting Started

1. **Clone the repo**:
   ```bash
   git clone https://github.com/your-username/IndieGameZone-Backend.git
   ```
2. **Run with .NET Aspire**:
   ```bash
   cd IndieGameZone.Backend
   dotnet run --project IndieGameZone.AppHost
   ```
   Access the Aspire dashboard at `http://localhost:18888`
4. **Docker(optional)**:
   ```bash
   docker build -t indiegamezone-api -f IndieGameZone.API/Dockerfile .
   docker run -p 8080:80 indiegamezone-api
   ```
   
## 📜 License

[MIT License](LICENSE) - See the license file for full details.

## 📚 Project Documentation

- [📊 ERD Diagram](docs/ERD.md)
- [🔌 API Endpoints](docs/API.md)
- [🧪 Testing Strategy](docs/TESTING.md)
- [🚀 Deployment Guide](docs/DEPLOYMENT.md)
- [📝 Code Style Guide](docs/STYLE_GUIDE.md)

## 🤝 Contributing

We welcome contributions! Please follow these guidelines:

1. **Fork** the repository
2. Create a **feature branch** (`git checkout -b feature/your-feature`)
3. **Commit** your changes (`git commit -m 'Add some feature'`)
4. **Push** to the branch (`git push origin feature/your-feature`)
5. Open a **Pull Request**

**Coding Standards:**
- Follow Clean Architecture principles
- Keep commits atomic and well-described
- Document new endpoints and services

## 👥 Development Team

| Student ID   | Name          | Role                | Responsibilities                  |
|--------------|---------------|---------------------|-----------------------------------|
| SE173551     | Trần Minh Tâm | Backend Lead        | API Development, Architecture     |
| DEF456       | Jane DevOps   | Infrastructure Lead | Docker, CI/CD Pipelines           |
| GHI789       | Alex QA       | Testing Specialist  | Unit/Integration Tests            |
| JKL012       | Sam DBA       | Database Engineer   | EF Core, Migrations               |

## 🔗 Related Links

- [📋 Project Board](https://github.com/your-org/IndieGameZone-Backend/projects/1)
- [🐛 Issue Tracker](https://github.com/your-org/IndieGameZone-Backend/issues)
- [📈 CI/CD Pipeline](https://dev.azure.com/your-org/_build)

---

Built with ❤️ by **IndieGameZone Team**  
📧 Contact: [team@indiegamezone.dev](mailto:team@indiegamezone.dev)
