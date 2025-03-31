
# ShelfSmart Project

**ShelfSmart** is a Smart Inventory Management System designed for pantry stock tracking, built as a capstone project. This repository serves as the parent project, integrating the frontend and backend as Git submodules. It streamlines inventory management with features like real-time tracking, alerts, and AI-driven suggestions.

## Submodules
- **[shelfsmart-frontend](https://github.com/MohitNamdev22/ShelfSmart-Backend)**: Frontend repository (React, Vite, Tailwind CSS).
- **[shelfsmart-backend](https://github.com/MohitNamdev22/ShelfSmart-Backend)**: Backend repository (Spring Boot, PostgreSQL).

## SRS Overview
Based on the Software Requirements Specification (SRS):
- **Purpose**: Streamline pantry inventory tracking and restocking.
- **Scope**: Developed in 2 weeks with CRUD operations, real-time tracking, alerts, and reports.
- **Must-Have Features**:
  - User registration, login, logout.
  - Inventory CRUD with stock movement tracking.
  - Low stock and expiry alerts.
  - Daily/weekly CSV reports.
- **Good-to-Have Features**:
  - Search/filter inventory.
  - Custom reports.
  - User activity log.
  - Supplier management.

## Tech Stack
- **Frontend**: React, Vite, Tailwind CSS, Axios, Chart.js
- **Backend**: Spring Boot 3.4.4, Java 17, PostgreSQL (NeonDB), Spring Security, Gemini API
- **Version Control**: Git & GitHub


## Prerequisites
- **Node.js**: v16.x+ (for frontend)
- **Java**: 17 (for backend)
- **Maven**: 3.6+ (for backend)
- **PostgreSQL**: NeonDB or local instance
- **Git**: For cloning and submodule management

## Installation
1. **Clone the Parent Repository with Submodules**:
   ```bash
   git clone --recurse-submodules https://github.com/your-username/shelfsmart-project.git
   cd shelfsmart-project

2.  Setup Frontend:
```bash
cd shelfsmart-frontend
npm install
echo "VITE_API_URL=http://localhost:8080" > .env
npm run dev
```

3.  Setup Backend:
```bash
cd ../shelfsmart-backend
mvn install`
Setup applicatiob.properties from application.properties.sample and add new Gemini API Key.
mvn spring-boot:run
```

4. Access the Application:
- Frontend: http://localhost:5173
- Backend: http://localhost:8080

5. Usage
- Start the backend first, then the frontend.
- Register/login to manage inventory, view reports, and receive alerts based on your role (Admin/User).

