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




