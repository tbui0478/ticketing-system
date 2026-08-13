# Ticketing-System
A full-stack IT help desk and ticketing platform inspired by tools like Jira Service Management and ServiceNow. It is built to demonstrate real-world software engineering practices including authentication, role-based access control, real-time updates, SLA tracking, and AI-assisted ticket triage.

>Status: In active development. This README will be updated with screenshots, final setup instructions, and a live demo link as features are completed.

---

# Overview
This project simulates a company's internal IT support desk. Employees ("Requesters") can submit tickets describing issues; IT staff ("Agents") triage, work, and resolve them; and "Admins" manage users, SLA policies, and view analytics which is similar to how real ITSM tools operate.

---

# Tech Stack

**Backend**
- Java 17 + Spring Boot 3
- Spring Security (JWT authentication)
- Spring Data JPA
- PostgreSQL
- WebSockets (real-time updates)
- Redis (caching / session support)
**Frontend**
- React (Vite)
- Recharts (analytics dashboard)
**DevOps**
- Docker & Docker Compose
- GitHub Actions (CI/CD)

---

## Planned Features
 
### Core
- [ ] User authentication & JWT-based sessions
- [ ] Role-based access control - Admin / Agent / Requester
- [ ] Create, view, update, and comment on tickets
- [ ] Ticket status workflow (Open → In Progress → Resolved → Closed)
- [ ] Priority levels (Low, Medium, High, Urgent)
### Differentiators
- [ ] **AI-powered ticket triage** - automatically suggests category, priority, and a short summary when a ticket is created
- [ ] **SLA tracking** - response/resolution timers per priority, with automatic breach detection and escalation
- [ ] **Real-time updates** - live ticket status changes and comments via WebSockets
- [ ] **Knowledge base with auto-suggestions** - recommends relevant articles as a user types a new ticket
- [ ] **Full audit trail** - every ticket field change is logged with who/when/what
### Polish
- [ ] Analytics dashboard - ticket volume, average resolution time, agent performance
- [ ] Kanban-style board view for agents
- [ ] Dark mode / responsive design
---
 
## Architecture
 
```
frontend/   → React app (dashboard, ticket views, auth)
backend/    → Spring Boot REST + WebSocket API
docker-compose.yml → Postgres, Redis, backend, frontend services
```
 
*(Architecture diagram to be added here once finalized.)*
 
---
 
## Getting Started
 
### Prerequisites
- Java 17+
- Node.js 18+
- Docker Desktop
- Maven
### Setup

# Clone the repo
git clone https://github.com/tbui0478/ticketing-system
cd ticketing-system
 
# Run everything with Docker Compose
docker compose up
```
 
*(Full setup instructions will be finalized as backend/frontend development progresses.)*
 
---
 
## Project Structure
 
```
helpdesk-ticketing-system/
├── backend/        # Spring Boot API
├── frontend/        # React app
├── docker-compose.yml
└── README.md
```
 
---
 
## Roadmap
 
- **Phase 1** — Core ticket CRUD, auth, RBAC
- **Phase 2** — SLA tracking, real-time updates, AI triage
- **Phase 3** — Analytics dashboard, knowledge base, UI polish
---
 
## Author
 
Built by Trinh Bui as a portfolio project to demonstrate full-stack development, system design, and modern engineering practices.


