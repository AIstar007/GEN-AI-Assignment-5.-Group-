# Crew Roster Optimization

This is a proof-of-concept for a crew rostering optimization system. It consists of a Python backend that handles the optimization logic and a React frontend for the user interface.

## Project Structure

The project is divided into two main parts:

- `frontend/`: A React application built with Vite that provides the user interface for interacting with the rostering system.
- `backend/`: A Python application that contains the core logic for data processing, rule enforcement, and roster optimization.

## Getting Started

### Prerequisites

- Node.js and npm (for the frontend)
- Python 3 and pip (for the backend)

### Installation

1. **Frontend:**
    ```bash
    cd frontend
    npm install
    ```

2. **Backend:**
    ```bash
    cd backend
    pip install -r requirements.txt
    ```

---

## Configuring React + Vite + TailwindCSS

We are using **TailwindCSS** with Vite for rapid UI development.  
Reference: [TailwindCSS + Vite Setup Guide](https://tailwindcss.com/docs/guides/vite)

### Steps:

1. **Create a Vite React app (if starting fresh):**
    ```bash
    npm create vite@latest frontend
    cd frontend
    npm install
    ```

2. **Install TailwindCSS and dependencies:**
    ```bash
    npm install -D tailwindcss postcss autoprefixer
    npx tailwindcss init -p
    ```

3. **Configure `tailwind.config.js`:**
    ```js
    /** @type {import('tailwindcss').Config} */
    export default {
      content: [
        "./index.html",
        "./src/**/*.{js,ts,jsx,tsx}",
      ],
      theme: {
        extend: {},
      },
      plugins: [],
    }
    ```

4. **Add Tailwind directives to `src/index.css`:**
    ```css
    @tailwind base;
    @tailwind components;
    @tailwind utilities;
    ```

5. **Run the dev server:**
    ```bash
    npm run dev
    ```

You should now have TailwindCSS working with React + Vite.

---

## Running the Application

1. **Start the backend server:**
    ```bash
    cd backend
    python main.py
    ```

2. **Start the frontend development server:**
    ```bash
    cd frontend
    npm run dev
    ```

---
