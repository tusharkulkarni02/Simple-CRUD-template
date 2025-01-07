# Simple-CRUD-template
Universal template to ease out building CRUD apps in MERN


***Here are the key commands to set up a MERN stack CRUD app:***

### 1. Initialize project and create directories:
```bash
mkdir mern-crud
cd mern-crud
mkdir backend frontend
```

### 2. Set up backend:
```bash
cd backend
npm init -y
npm install express mongoose cors dotenv nodemon
```
- express: Web framework
- mongoose: MongoDB object modeling
- cors: Enable cross-origin requests
- dotenv: Environment variables
- nodemon: Auto-restart server during development

### 3. Set up frontend:
```bash
cd ../frontend
npx create-react-app .
npm install axios react-router-dom
```
- create-react-app: Creates React project structure
- axios: HTTP client for API requests
- react-router-dom: Client-side routing

### 4. Add scripts to backend package.json:
```json
"scripts": {
  "start": "node server.js",
  "dev": "nodemon server.js"
}
```

### The basic structure will be:
```
mern-crud/
  ├── backend/
  │   ├── models/
  │   ├── routes/
  │   ├── server.js
  │   └── .env
  └── frontend/
      ├── src/
      ├── public/
      └── package.json
```

### Start development with:
```bash
# Terminal 1 (backend)
cd backend
npm run dev

# Terminal 2 (frontend)
cd frontend
npm start
```
