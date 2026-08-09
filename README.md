# 🗄️ Valhalla Gym - Database Architecture & Infrastructure (`valhalla-db`)

A high-performance, scalable PostgreSQL schema and Redis caching setup designed for **Valhalla Gym Management System**. Built with multi-tenancy (white-label capability) in mind to support seamless rebranding for future commercialization.

---

## 🛠️ Tech Stack & Infrastructure

- **Database Engine:** PostgreSQL 16
- **In-Memory Cache:** Redis 7
- **Containerization:** Docker & Docker Compose
- **Scripting:** Pure SQL (DDL + Performance Indexing)

---

## 📐 Schema Overview & Features

- 🏢 **White-Label Configuration:** Global `gym_config` table for dynamic branding, currency, and custom themes.
- 👤 **Role-Based Access Control (RBAC):** Native Enum types for `SUPERADMIN`, `ADMIN`, `TRAINER`, and `MEMBER`.
- ⚡ **High-Throughput Check-Ins:** Indexed schema optimized for fast QR token lookup and Redis caching.
- 🤖 **AI Routine Storage:** JSONB columns for flexible AI-generated workout and nutrition plans.
- 🔒 **UUID Identifiers:** Primary keys powered by `uuid-ossp` extension to ensure data security and avoid sequential ID exposure.

---

## 🚀 Quick Start (Local Setup)

### Prerequisites
- [Docker Desktop](https://www.docker.com/products/docker-desktop/) installed and running.

### Execution
1. Clone the repository:
   ```bash
   git clone [https://github.com/OdiazLz/valhalla-db.git](https://github.com/OdiazLz/valhalla-db.git)
   cd valhalla-db