# Enterprise-Microservices-Base-Architecture

A professional-grade **Monorepo** template designed for high-scale enterprise solutions. This repository provides a **Microservices Base Architecture** using **Clean Architecture** principles, integrating a powerful **.NET 10** backend with a modern **Next.js 16.1** frontend.

## 📂 Full Project Structure

<details>
<summary><b>Click to expand the complete directory tree</b></summary>

```text
.
├── apps
│   ├── backend
│   │   ├── auth
│   │   │   ├── Applications
│   │   │   ├── AuthService.slnx
│   │   │   ├── Domain
│   │   │   │   ├── AuthService.Domain.csproj
│   │   │   │   ├── Class1.cs
│   │   │   │   ├── Entities
│   │   │   │   ├── Models/Filters
│   │   │   │   ├── Repositories
│   │   │   │   └── obj
│   │   │   │       ├── AuthService.Domain.csproj.nuget.dgspec.json
│   │   │   │       ├── AuthService.Domain.csproj.nuget.g.props
│   │   │   │       ├── AuthService.Domain.csproj.nuget.g.targets
│   │   │   │       ├── project.assets.json
│   │   │   │       └── project.nuget.cache
│   │   │   ├── Infrastructure
│   │   │   │   ├── AuthService.Infrastructure.csproj
│   │   │   │   ├── Caching
│   │   │   │   ├── Class1.cs
│   │   │   │   ├── Config
│   │   │   │   ├── Data/Migrations
│   │   │   │   ├── DependencyInjection
│   │   │   │   ├── Graphql
│   │   │   │   ├── Logging
│   │   │   │   ├── Repositories
│   │   │   │   ├── Startup
│   │   │   │   └── obj
│   │   │   │       ├── AuthService.Infrastructure.csproj.nuget.dgspec.json
│   │   │   │       ├── AuthService.Infrastructure.csproj.nuget.g.props
│   │   │   │       ├── AuthService.Infrastructure.csproj.nuget.g.targets
│   │   │   │       ├── project.assets.json
│   │   │   │       └── project.nuget.cache
│   │   │   ├── Presentation
│   │   │   │   ├── AuthService.Presentation.csproj
│   │   │   │   ├── Program.cs
│   │   │   │   ├── Properties
│   │   │   │   │   └── launchSettings.json
│   │   │   │   ├── Graphql
│   │   │   │   │   ├── Http
│   │   │   │   │   ├── Inputs
│   │   │   │   │   ├── SignalR
│   │   │   │   │   └── Types
│   │   │   │   ├── appsettings.Development.json
│   │   │   │   ├── appsettings.json
│   │   │   │   └── obj
│   │   │   │       ├── AuthService.Presentation.csproj.nuget.dgspec.json
│   │   │   │       ├── AuthService.Presentation.csproj.nuget.g.props
│   │   │   │       ├── AuthService.Presentation.csproj.nuget.g.targets
│   │   │   │       ├── project.assets.json
│   │   │   │       └── project.nuget.cache
│   │   │   ├── Properties
│   │   │   ├── Scripts
│   │   │   └── Security/Jwt
│   │   └── exchange
│   │       ├── Applications
│   │       │   ├── Class1.cs
│   │       │   ├── Errors
│   │       │   ├── ExchangeService.Applications.csproj
│   │       │   ├── Services
│   │       │   └── obj
│   │       │       ├── ExchangeService.Applications.csproj.nuget.dgspec.json
│   │       │       ├── ExchangeService.Applications.csproj.nuget.g.props
│   │       │       ├── ExchangeService.Applications.csproj.nuget.g.targets
│   │       │       ├── project.assets.json
│   │       │       └── project.nuget.cache
│   │       ├── Domain
│   │       │   ├── Class1.cs
│   │       │   ├── Entities
│   │       │   ├── ExchangeService.Domain.csproj
│   │       │   ├── Models/Filters
│   │       │   ├── Repositories
│   │       │   └── obj
│   │       │       ├── ExchangeService.Domain.csproj.nuget.dgspec.json
│   │       │       ├── ExchangeService.Domain.csproj.nuget.g.props
│   │       │       ├── ExchangeService.Domain.csproj.nuget.g.targets
│   │       │       ├── project.assets.json
│   │       │       └── project.nuget.cache
│   │       ├── ExchangeService.slnx
│   │       ├── Infrastructure
│   │       │   ├── Caching
│   │       │   ├── Class1.cs
│   │       │   ├── Config
│   │       │   ├── Data/Migrations
│   │       │   ├── DependencyInjection
│   │       │   ├── ExchangeService.Infrastructure.csproj
│   │       │   ├── Graphql
│   │       │   ├── Logging
│   │       │   ├── Repositories
│   │       │   ├── Startup
│   │       │   └── obj
│   │       ├── Presentation
│   │       │   ├── ExchangeService.Presentation.csproj
│   │       │   ├── Graphql
│   │       │   │   ├── Http
│   │       │   │   ├── Inputs
│   │       │   │   ├── SignalR
│   │       │   │   └── Types
│   │       │   ├── Program.cs
│   │       │   ├── Properties
│   │       │   │   └── launchSettings.json
│   │       │   ├── appsettings.Development.json
│   │       │   ├── appsettings.json
│   │       │   └── obj
│   │       │       ├── ExchangeService.Presentation.csproj.nuget.dgspec.json
│   │       │       ├── ExchangeService.Presentation.csproj.nuget.g.props
│   │       │       ├── ExchangeService.Presentation.csproj.nuget.g.targets
│   │       │       ├── project.assets.json
│   │       │       └── project.nuget.cache
│   │       ├── Properties
│   │       ├── Scripts
│   │       └── Security/Jwt
│   └── frontend
│       ├── admin
│       │   ├── .gitignore
│       │   ├── .next
│       │   ├── README.md
│       │   ├── eslint.config.mjs
│       │   ├── next-env.d.ts
│       │   ├── next.config.ts
│       │   ├── node_modules
│       │   ├── package.json
│       │   ├── public
│       │   │   ├── file.svg
│       │   │   ├── globe.svg
│       │   │   ├── next.svg
│       │   │   ├── vercel.svg
│       │   │   └── window.svg
│       │   ├── src
│       │   │   └── app
│       │   │       ├── favicon.ico
│       │   │       ├── globals.css
│       │   │       ├── layout.tsx
│       │   │       ├── page.module.css
│       │   │       └── page.tsx
│       │   ├── tsconfig.json
│       │   └── yarn.lock
│       └── web
│           ├── .gitignore
│           ├── .next
│           ├── README.md
│           ├── eslint.config.mjs
│           ├── next-env.d.ts
│           ├── next.config.ts
│           ├── node_modules
│           ├── package.json
│           ├── public
│           │   ├── file.svg
│           │   ├── globe.svg
│           │   ├── next.svg
│           │   ├── vercel.svg
│           │   └── window.svg
│           ├── src
│           │   └── app
│           │       ├── favicon.ico
│           │       ├── globals.css
│           │       ├── layout.tsx
│           │       ├── page.module.css
│           │       └── page.tsx
│           ├── tsconfig.json
│           └── yarn.lock
├── libs
│   ├── contracts
│   │   └── src
│   │       ├── auth
│   │       └── common
│   ├── graphql
│   │   ├── documents
│   │   │   ├── admin
│   │   │   └── web
│   │   ├── generated
│   │   │   ├── auth
│   │   │   └── exchange
│   │   └── schema
│   └── ui
│       └── src
│           ├── components
│           ├── icons
│           ├── layouts
│           └── styles
├── .gitignore
├── env.example
└── README.md
```
</details>

🏗 Architecture & Design
This project is built to demonstrate a true enterprise environment where scalability and maintainability are top priorities.

🔹 Microservices (Backend)
Located in apps/backend/, each service follows the Clean Architecture (Domain, Application, Infrastructure, Presentation) pattern:

Auth Service: Handles Identity, JWT-based security, and user management.

Exchange Service: Manages core business logic, transactions, and market data.

Unified GraphQL: Built with HotChocolate to provide a single, typed API entry point.

🔹 Applications (Frontend)
Located in apps/frontend/, using Next.js 15 and TypeScript:

Admin Dashboard: Dedicated portal for system administrators.

Web Portal: Public-facing application with optimized performance and SEO.

🔹 Shared Core (libs)
Contracts: Unified DTOs and shared communication protocols.

UI Library: A shared React component library for design consistency across all apps.

GraphQL Tools: Auto-generated hooks and types for seamless API integration.

🛠 Tech Stack
Backend: .NET 10, EF Core, HotChocolate (GraphQL), SignalR.

Frontend: Next.js 16.1 (App Router), Tailwind CSS, TypeScript.

Database: PostgreSQL / SQL Server.

DevOps: Monorepo structure for simplified CI/CD and dependency management.

🚀 Installation & Usage
Clone the repository:
```
git clone [https://github.com/mratashnejad/enterprise-microservices-base.git](https://github.com/mratashnejad/enterprise-microservices-base.git)
cd enterprise-microservices-base
```

Backend Setup (.NET 10):
Navigate to the desired service to restore dependencies and run the project.
```
cd apps/backend/auth/Presentation
dotnet restore
dotnet run
```
Frontend Setup (Next.js 16.1):
Navigate to the frontend applications to install packages and start the development server.
```
cd ../../../../apps/frontend/web
yarn install
yarn dev
```

🛡 License
This project is licensed under the MIT License.
