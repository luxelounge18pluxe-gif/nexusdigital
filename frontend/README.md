# AI Tools Marketplace - Backend Scaffold

This project provides a minimal Node.js/Express backend scaffold for the static frontend files in this workspace (`ai tool.html` and `admin/admin.html`).

What was added
- `server.js` — Express server exposing a simple REST API under `/api/tools` and serving static frontend files.
- `package.json` — with `express` and `cors` dependencies and `start`/`dev` scripts.
- `data/tools.json` — persistent JSON storage for tools.
- `.gitignore` — ignoring `node_modules` and uploads.

Quick start

1. Open a terminal in the project root (where `package.json` is located).

2. Install packages:

```bash
npm install
```

3. Start the server:

```bash
npm start
```

4. Open the frontend in your browser:

- Main app: http://localhost:3000/ai%20tool.html
- Admin panel: http://localhost:3000/admin/admin.html

Notes
- The backend stores tools in `data/tools.json`. It supports standard CRUD via `/api/tools`.
- Current frontend uses localStorage; if you want I can wire `admin/admin.html` and `ai tool.html` to use these API endpoints instead of localStorage.
