# CampusBuddy-SE

##  Project Overview
CampusBuddy is a hostel & campus support system that helps students raise complaints, track issues, and receive hostel services smoothly.

##  Problem Statement
In many hostels, complaints like maintenance issues, mess feedback, and parcel updates are handled manually (WhatsApp calls, registers, repeated follow-ups).  
This causes delays, confusion, and no proper tracking.

##  Target Users (Personas)
- Hostel Students
- Warden / Admin
- Maintenance Staff
- Mess Manager (optional)

##  Key Features
- Student login and profile
- Raise complaint with category + description + photo
- Track complaint status (Pending → Assigned → In Progress → Completed)
- Warden assigns tasks to staff
- Staff updates progress
- Mess feedback system
- Monthly report generation

##  Success Metrics
- Reduced complaint resolution time
- Fewer repeated complaints
- Higher student satisfaction

##  Assumptions & Constraints
- Only college/hostel students can register
- Internet connection is needed
- Basic smartphone/web access is available

##  Repository Structure
- `docs/` → MoSCoW, project documentation  
- `wireframes/` → Figma wireframe screenshots  
- `architecture/` → Architecture diagram  
- `screenshots/` → Proof screenshots (Docker/GitHub working)
  
##  Branching Strategy
This project follows GitHub Flow:
- `main` branch contains stable code
- Feature updates are done in separate branches like `feature/*`
- Changes are merged back into `main` after completion
  
##  Quick Start – Local Development (Docker)

### 1) Build Docker image
```bash
docker build -t campusbuddy-se .
docker run -p 8080:80 campusbuddy-se

---

## 🏗️ Software Design

The CampusBuddy system follows a layered client–server architecture to ensure scalability, modularity, and maintainability. The design separates the presentation layer, application logic, data storage, and deployment infrastructure.

### 📌 High-Level Architecture

The system consists of:

- **Frontend Layer** (Student, Warden, Maintenance Interfaces)
- **Backend API Layer** (Authentication, Complaint Management, Notification Modules)
- **Database Layer** (MySQL for structured data)
- **Cloud Storage** (For complaint image uploads)
- **Infrastructure Layer** (Docker-based containerized deployment)

📎 Architecture Diagram:  
`docs/design/architecture.png`

---

### 🎨 User Interface Design

The user interface was designed using Figma and focuses on:

- Consistent layout and button styles  
- Clear form inputs and labels  
- Status visibility (Pending, In Progress, Completed)  
- Role-based dashboards  
- Mobile-friendly vertical layout  

📎 UI Screens:  
`docs/design/ui-screens.png`

---

### ⚙️ Key Design Decisions

1. Separation of frontend and backend for low coupling.
2. Modular backend structure for maintainability.
3. Role-Based Access Control (RBAC) for security.
4. Docker containerization for consistent deployment.
5. Cloud storage for scalable complaint image handling.

These decisions improve system scalability, security, and long-term maintainability.

---


