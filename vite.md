# Template using Vite
---
*** Contains downloadable packages for auth as well! ***
### Project Setup:
```bash
# Create project
npm create vite@latest mern-project
cd mern-project
mkdir backend frontend
```

### Frontend Setup (/frontend):
```bash
# Initial setup
cd frontend
npm install

# Essential packages
npm i react-router-dom @reduxjs/toolkit react-redux axios
npm i @mui/material @emotion/react @emotion/styled 
npm i -D sass eslint prettier

# Development
npm run dev
```

### Backend Setup (/backend):
```bash
# Initialize
cd backend
npm init -y

# Core packages
npm i express mongoose cors dotenv
npm i bcryptjs jsonwebtoken helmet
npm i -D nodemon

# Development
npm run dev
```

### Project Structure:
```
mern-project/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── store/
│   │   ├── utils/
│   │   └── App.jsx
│   └── package.json
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   └── package.json
└── .gitignore
```

### Root package.json:
```json
{
  "scripts": {
    "start": "node backend/server.js",
    "server": "nodemon backend/server.js",
    "client": "npm run dev --prefix frontend",
    "dev": "concurrently \"npm run server\" \"npm run client\""
  }
}
```

### Environment Setup:
```bash
# Frontend (.env)
VITE_API_URL=http://localhost:5000

# Backend (.env)
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_secret
```
