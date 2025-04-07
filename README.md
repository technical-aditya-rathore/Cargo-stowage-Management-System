# Cargo Stowage Management System

A smart cargo placement, retrieval, and simulation system developed for the *National Space Hackathon 2025*.

---

## Features
- *Optimal Cargo Placement* using greedy + heuristic strategies
- *Real-time Search & Retrieval* of cargo items
- *Waste Management*: Identify and manage unplaced cargo
- *Reorganization & Rearrangement* based on priority
- *Simulation of Time*: Auto-behavior simulation across days
- *Dockerized & API-Driven*: Easy to deploy, use, and test

---

## Technology Stack
- *Backend*: FastAPI (Python)
- *Frontend*: React + TailwindCSS
- *Containerization*: Docker (Ubuntu 22.04)

---

## Setup Instructions

### Backend
bash
# Clone repo and navigate into it
git clone https://github.com/technical-aditya-rathore/cargo-stowage.git
cd cargo-stowage
and original readme is:- https://github.com/technical-aditya-rathore/Cargo-stowage-Management-System/edit/main/README.md

# Build Docker image
docker build -t cargo-stowage .

# Run container
docker run -p 8000:8000 cargo-stowage

Access API at: http://localhost:8000/docs

---

### Frontend (Optional - if using UI)
bash
cd frontend
npm install
npm run dev

Access UI at: http://localhost:3000

---

## API Reference (Backend)

| Endpoint | Method | Description |
|----------|--------|-------------|
| /api/import/containers | POST | Import list of containers |
| /api/import/items | POST | Import list of items |
| /api/search | GET | Search item by name |
| /api/place | POST | Place items in containers optimally |
| /api/retrieve | POST | Retrieve a specific item |
| /api/waste/identify | GET | Identify waste items |
| /api/waste/return-plan | POST | Return plan for waste items |
| /api/waste/complete-undocking | POST | Remove waste permanently |
| /api/simulate/day | POST | Simulate a single time unit |
| /api/export/arrangement | GET | Export current container arrangement |
| /api/logs | GET | View system logs |

---

## Sample Data
Use sample_data/items.json and sample_data/containers.json provided in the repo for testing.

---

## License
This project is for educational and competitive use under the National Space Hackathon 2025.

---

## Authors
- Team Name:- Creating Specific
- [Aditya Kumar Jha] (Team Leader)
- [Aditya  Kumar Jha]
- [solo no other members] (if any)
