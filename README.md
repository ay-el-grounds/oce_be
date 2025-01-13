# Oil Change, Etc. Backend (`oce_be`)

This repository contains the backend services for **Oil Change, Etc.**, including API integrations, Firebase functionality, and middleware for handling user data.

## Features
- Firebase Admin SDK for user data and authentication.
- Integration with DIMO Telemetry API for real-time vehicle data.
- RESTful API for handling vehicle profiles, maintenance logs, and more.

## Getting Started
### Prerequisites
- Node.js v16+
- Firebase project credentials (`serviceAccountKey.json`)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/ay-el-grounds/oce_be.git
   cd oce_be
   ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Add a .env file with the following:
    ```makefile
    PORT=5000
    ```
4. Start the server:
    ```bash
    npm run dev
    ```

### Folder Structure
```plaintext
oce_be/
├── src/
│   ├── functions/       # Firebase Cloud Functions
│   ├── integrations/    # API integrations (e.g., DIMO, external APIs)
│   ├── middlewares/     # Custom middleware for API requests
│   ├── models/          # Data models
│   ├── routes/          # Backend routes
│   ├── utils/           # Utility functions
│   └── index.js         # Main entry point
├── .gitignore           # Ignore unnecessary files
├── package.json         # Project dependencies
├── README.md            # Documentation for backend
```

---

### API Endpoints
GET /: Health check for the backend.
POST /vehicle: Add a new vehicle profile.
GET /vehicle/:id: Fetch a vehicle profile.

---

### License
This project is licensed under the MIT License.