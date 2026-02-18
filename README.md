# OpenField ⚽ | Autonomous Sports Predictive Engine

> **Status:** 🚧 In Development (Architecture Phase)
> **Tech Stack:** .NET 10 (LTS) | C# 14

## 🎯 Vision

OpenField is not just a prediction tool; it is a **High-Performance Autonomous Engine** designed to process complex sports data. Unlike traditional betting scripts, OpenField utilizes **Clean Architecture** and **Domain-Driven Design (DDD)** to create a platform agnostic to specific championships (Multi-League Support).

The system is designed to "self-feed" via resilient background workers, process data using statistical models (Poisson Distribution + Machine Learning), and deliver real-time probabilities with high reliability.

## 🏗 Architecture & Tech Stack

The project is built on the latest **.NET 10** ecosystem, leveraging **C# 14** features for maximum performance and expressiveness.

- **Core:** Pure C# 14 Logic. Implements rich Domain Models and Strategy Patterns.
- **Application:** CQRS orchestration.
- **Infrastructure:**
  - **Data:** EF Core 10 & Dapper. optimized for high-throughput writes and low-latency reads.
  - **Integrations:** Resilient scraping with Polly.
- **Presentation:**
  - **Web API:** .NET 10 Minimal APIs / Controllers.
  - **Worker Service:** Native AOT-ready background agents.

## 🚀 Key Features (Roadmap)

- [ ] **Multi-League Engine:** Configurable RuleSets.
- [ ] **Resilient ETL:** Fault-tolerant ingestion pipelines.
- [ ] **Predictive Core:** Poisson Distribution & ML.NET integration.
- [ ] **Event Sourcing (Planned):** Temporal data tracking.

## 🤝 How to contribute

This is an **Open Source** project. If you love football, statistics, or want to practice the latest features of the .NET ecosystem, you are welcome to:

1. Open **Issues** with suggestions for new model variables.
2. Contribute code via **Pull Requests**.
3. Improve the technical documentation.

## 📄 License

This project is licensed under the **GNU General Public License v3.0 (GPLv3)**. See the [`LICENSE`](LICENSE) file for more details.

By adopting this license, we ensure that **OpenField** and any improvements made by third parties remain open and free for the community.

## 🛠 How to Run

_Requires .NET 10 SDK and SQL Server/Docker._

1. Clone the repo.
2. Update connection strings in `appsettings.json`.
3. Run `dotnet ef database update`.
4. Launch the Worker Service.

---

_Developed with ❤️ by **Bruno Gabriel Knop**._
