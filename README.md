# Jagdamba Optical Backend + Admin Panel

## Features
- Node.js + Express REST API
- MongoDB Atlas database
- JWT admin login
- Product CRUD (add/edit/hide)
- Enquiry management
- Store settings management
- Dashboard counts
- Existing frontend connected to the API
- Admin panel included in `frontend/admin.html`

## 1. Install
```bash
cd backend
npm install
```

## 2. MongoDB
Create a free MongoDB Atlas cluster and database. Add your IP/network access and copy the connection string.

## 3. Environment
Copy `.env.example` to `.env` and fill:
- MONGODB_URI
- JWT_SECRET
- ADMIN_EMAIL
- ADMIN_PASSWORD
- FRONTEND_URL

## 4. Run backend
```bash
npm run dev
```
API: `http://localhost:5000`

## 5. Run frontend
Use VS Code Live Server or:
```bash
cd frontend
python -m http.server 5500
```
Open `http://localhost:5500`.

Admin:
`http://localhost:5500/admin.html`

## Important
Change the default admin password before publishing.
The product `image` field accepts an image URL. For production image uploads, connect Cloudinary/S3 later.
