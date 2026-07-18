<h1 align="center">🔐 Secure File Share</h1>
<p align="center">Upload a file, get a code, share it anywhere — retrieve it on any device, no account required.</p>

<p align="center">
  <a href="https://eco-stemm-ewx3.vercel.app"><img src="https://img.shields.io/badge/Live%20Demo-Visit%20App-46E3B7?style=for-the-badge" /></a>
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white" />
  <img src="https://img.shields.io/badge/Cloudinary-3448C5?style=for-the-badge&logo=cloudinary&logoColor=white" />
</p>

---

##  About

**Secure File Share** is a cross-device file sharing web app. Upload a file from any device, and the app generates a unique 6-character access code. Share that code with anyone, and they can retrieve and download the file from any other device — no account, no app install, just the code.

Built as a full-stack project with a React frontend and an Express.js backend, using Cloudinary for cloud file storage.

## Features

**JWT-based authentication** — secure login/signup with bcrypt password hashing
**Drag & drop file upload** — with Cloudinary cloud storage under the hood
**Unique access codes** — share a code instead of a link or login
**Cross-device retrieval** — upload on one device, download on any other (phone, laptop, tablet)
**File management** — star important files, track recent uploads
**Works everywhere** — any browser, any device, any network

##  Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React, Framer Motion, Lucide Icons |
| Backend | Express.js, JWT, bcrypt |
| Storage | Cloudinary |
| Deployment | Vercel (frontend) | Render (Backend) |

##  Getting Started

### Prerequisites
- Node.js and npm installed

### Installation

```bash
git clone https://github.com/sahilroyal07/ecosystem-file-share.git
cd ecosystem-file-share
npm install
```

### Run locally

```bash
# Option 1: use the start script
./start.sh

# Option 2: start manually
npm run dev
```

- Frontend: `http://localhost:3000`
- Backend API: `http://localhost:5000`

### Environment variables

Create a `.env` file (see `.env.example`) with:

```
REACT_APP_CLOUDINARY_URL=https://api.cloudinary.com/v1_1/<your-cloud-name>/upload
REACT_APP_UPLOAD_PRESET=<your-upload-preset>
REACT_APP_API_URL=http://localhost:5000
JWT_SECRET=your-super-secret-jwt-key-change-in-production
PORT=5000
```

##  How It Works

1. **Upload** a file from any device — get a unique access code (e.g. `ABC123`)
2. **Share** the code via text, email, or chat
3. **Retrieve** the file on any other device using the code — no login needed

## 📂 Project Structure

```
secure-file-share/
├── src/
│   ├── components/
│   │   └── MainApp.js        # Main application component
│   ├── services/
│   │   └── fileService.js    # Frontend API service layer
│   ├── App.js
│   ├── App.css
│   └── config/
│       └── environment.js
├── backend/
│   └── api/
│       └── server.js         # Backend API
└── server/                   # Legacy server files
```

## 📄 Documentation

More detail is available in this repo:
- `SETUP.md` — setup & quick start guide
- `USAGE_GUIDE.md` — cross-device usage walkthrough
- `DEPLOYMENT.md` — deployment instructions
- `STRUCTURE.md` — project structure notes

## 🔗 Live Demo

 [eco-stemm-ewx3.vercel.app](https://eco-stemm-ewx3.vercel.app)

---
