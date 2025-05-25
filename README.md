# 🚀 GitHub to Azure CI Pipeline Migration: Voting App Modernization

This project demonstrates my experience **migrating GitHub-based CI pipelines to Azure DevOps** by containerizing and orchestrating a multi-language voting application using **Docker** and **Azure DevOps Pipelines**.

The voting app is a microservices-based architecture, consisting of:

- 🗳️ **Vote App** (Python Flask): Accepts one-time client votes between two options.
- 📊 **Result App** (Node.js): Displays real-time voting results.
- ⚙️ **Worker App** (.NET Core): Consumes votes from Redis and stores them in PostgreSQL.
- 🐘 **PostgreSQL**: Persists voting results.
- 🧠 **Redis**: Queues incoming votes.

---

## 🔧 Project Goal

> **Migrate CI pipelines from GitHub Actions to Azure DevOps Pipelines** for a containerized microservices-based application.

---

## 🛠️ My Contributions

✅ Migrated CI pipelines for each service (`vote`, `worker`, and `result`) from GitHub Actions to **Azure Pipelines**  
✅ Created **3 independent Azure DevOps Pipelines** for building and pushing Docker images:
- **Vote Pipeline**: Python-based front-end
- **Worker Pipeline**: .NET Core background processor
- **Result Pipeline**: Node.js result dashboard

✅ Used **Azure DevOps YAML-based pipelines** to automate:
- Code checkout from GitHub
- Docker image build
- Push to Azure Container Registry (ACR)
  
✅ Ensured pipeline reusability and modularity via templated YAML structures  
✅ Verified end-to-end deployment with live vote updates across all services

---

## 🧱 Tech Stack

| Area         | Tech Used |
|--------------|-----------|
| CI/CD        | Azure DevOps Pipelines |
| Containers   | Docker, Docker Compose |
| Languages    | Python, Node.js, .NET Core |
| Messaging    | Redis |
| Database     | PostgreSQL |
| Hosting      | Azure Container Registry (ACR), Local Docker |

---

## 📁 Repository Structure

