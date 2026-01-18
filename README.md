## How to Launch the Application

This application consists of a **Backend** (Express.js) and **Frontend** (React) that need to be run separately. Follow the steps below to get both running.

### Prerequisites
- **Node.js** (v14 or higher) and **npm** installed on your machine
- Two terminal windows/tabs available (one for backend, one for frontend)

---

### Step 1: Install Dependencies

#### Backend Dependencies
1. Open a terminal and navigate to the backend directory:
   ```bash
   cd StarterCode/backend
   ```
2. Install backend dependencies:
   ```bash
   npm install
   ```
   This will install: `express`, `cors`, `dotenv`, and `nodemon`

#### Frontend Dependencies
1. Open a terminal (can be the same one after backend install, or a new one) and navigate to the frontend directory:
   ```bash
   cd StarterCode/frontend
   ```
2. Install frontend dependencies:
   ```bash
   npm install
   ```
   This will install: `react`, `axios`, `@mui/material`, and other React dependencies.

---

### Step 2: Launch the Backend Server

1. **Navigate to the backend directory** (if not already there):
   ```bash
   cd StarterCode/backend
   ```

2. **Start the backend server**:
   ```bash
   node index.js
   ```

   **Alternative (with auto-restart on file changes):**
   ```bash
   npx nodemon index.js
   ```

3. **Verify the backend is running:**
   - You should see: `Server is running on port 5000`
   - The backend API will be available at: `http://localhost:5000`
   - You can test it by visiting: `http://localhost:5000/api/products` in your browser

4. **Keep this terminal window open** - the backend server must continue running.

---

### Step 3: Launch the Frontend Application

1. **Open a NEW terminal window/tab** (keep the backend terminal running)

2. **Navigate to the frontend directory**:
   ```bash
   cd StarterCode/frontend
   ```

3. **Start the React development server**:
   ```bash
   npm start
   ```

4. **The frontend will automatically:**
   - Start on `http://localhost:3000`
   - Open in your default web browser
   - Hot-reload when you make code changes

---

### Step 4: Verify Everything is Working

1. **Check Backend:**
   - Backend terminal shows: `Server is running on port 5000`
   - Visit `http://localhost:5000/api/products` in browser - should show JSON data

2. **Check Frontend:**
   - Browser automatically opened to `http://localhost:3000`
   - You should see product cards displayed with:
     - Product name
     - Product description  
     - Product price
     - Product image
     - Delete icon button on each card

3. **Test Functionality:**
   - Products should load from the backend
   - Click the delete icon on any product card - it should disappear
   - Refresh the page (F5) - deleted products should remain deleted

---

### 🛑 How to Stop the Servers

**Backend Server:**
- In the backend terminal, press `Ctrl + C` (or `Cmd + C` on Mac)

**Frontend Server:**
- In the frontend terminal, press `Ctrl + C` (or `Cmd + C` on Mac)

---

### 📝 Quick Reference

| Service | Directory | Command | Port | URL |
|---------|-----------|---------|------|-----|
| Backend | `StarterCode/backend` | `node index.js` | 5000 | http://localhost:5000 |
| Frontend | `StarterCode/frontend` | `npm start` | 3000 | http://localhost:3000 |


