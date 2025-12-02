# 🚀 How to Run This Project Locally

Follow the steps below to set up and run this POS system on your local machine.

---

## 📥 1. Clone the Repository
\
   git clone https://github.com/<your-username>/<your-repo-name>.git
   cd <your-repo-name>


---

## 🛠️ 2. Run the Backend (Spring Boot)

### Prerequisites
- Java 17 or higher  
- Maven  
- MySQL Server  

### Steps
1. Create a MySQL database:
    \`\`\`sql
    CREATE DATABASE pos_system;
    \`\`\`

2. Update MySQL username/password in:
    \`\`\`
    pos-backend/src/main/resources/application.yml
    \`\`\`

3. Start the backend:
    \`\`\`sh
    cd pos-backend
    mvn spring-boot:run
    \`\`\`

Backend will start at:  
\`\`\`
http://localhost:8080
\`\`\`

---

## 🖥️ 3. Run the Frontend (React + Vite)

### Prerequisites
- Node.js (16+)
- npm or yarn

### Steps
1. Install dependencies:
    \`\`\`sh
    cd pos-frontend
    npm install
    \`\`\`

2. Start the dev server:
    \`\`\`sh
    npm run dev
    \`\`\`

Frontend will run at:  
\`\`\`
http://localhost:5173
\`\`\`

---

## 🔗 Connecting Frontend & Backend
Frontend connects to:  
\`\`\`
http://localhost:8080
\`\`\`

To change backend URL:  
\`\`\`
pos-frontend/src/config/api.js
\`\`\`

---

## 📁 Project Structure
\`\`\`
.
├── pos-backend/         # Spring Boot backend
└── pos-frontend/        # React frontend
\`\`\`

---

## ✔️ Done!
You now have both backend and frontend running locally.
