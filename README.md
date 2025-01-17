# MERN Starter Template

Welcome to the MERN Starter Template! This template is designed to help you kickstart your projects with a robust and modern setup that includes all the essentials.

## Features

### **Frontend**
- **Light and Dark Mode**: Built-in methods for toggling light and dark themes.
- **Authentication**:
  - Login and Signup pages.
  - Password recovery with OTP verification via email.
  - JWT-based authentication.
- **React Router**: Pre-configured for seamless navigation.
- **State Management**: Configured with Zustand for efficient global state handling.
- **ShadCN and Tailwind CSS**: Preconfigured for styling and design consistency.
- **React Hook Form**: Simplifies form handling with validations.
- **React Icons**: Easily add icons to your components.

### **Backend**
- **Express.js**: A REST API setup with routing, controllers, and models.
- **Authentication**:
  - JWT-based authentication for secure endpoints.
  - Nodemailer integrated for email services (OTP verification and password recovery).
- **Socket.io**: Real-time communication enabled.
- **Cloudinary Integration**: For image uploads and storage.
- **Environment Variables**: Configured with `dotenv` for secure key management.
- **Database**: MongoDB with Mongoose schemas and models.

### **Additional Configurations**
- **TypeScript**: Type-safe codebase for both frontend and backend.
- **Axios**: Pre-configured for API requests.
- **CORS**: Ensures cross-origin request safety.

## Environment Variables

### **Backend**
```env
PORT=8000
ENVIRONMENT=development

MONGODB_URI=""

ACCESS_TOKEN_SECRET=""
ACCESS_TOKEN_EXPIRY=1d
REFRESH_TOKEN_SECRET=""
REFRESH_TOKEN_EXPIRY=10d

HTTP_SECURE_OPTION=true
ACCESS_CONTROL_ORIGIN=http://localhost:5173 # For React app

CLOUDINARY_CLOUD_NAME=""
CLOUDINARY_API_KEY=""
CLOUDINARY_API_SECRET=""

GMAIL_APP_PASSWORD=""
GMAIL_USER=""
```

### **Frontend**
```env
VITE_SERVER_ORIGIN=http://localhost:8000 
VITE_SERVER_API_URL=http://localhost:8000/api/v1
VITE_ACCESS_CONTROL_ORIGIN=http://localhost:5173
```

## Folder Structure

```
mern-starter-template/
├── README.md
├── client/
│   ├── components.json
│   ├── index.html
│   ├── package.json
│   ├── .env
│   ├── public/
│   └── src/
│       ├── App.css
│       ├── App.tsx
│       ├── index.css
│       ├── main.tsx
│       ├── Hooks/
│       ├── assets/
│       │   └── Oswald/
│       │       ├── Oswald-VariableFont_wght.ttf
│       │       └── static/
│       ├── components/
│       │   ├── Forms/
│       │   ├── general/
│       │   └── ui/
│       ├── constants/
│       │   └── appName.ts
│       ├── pages/
│       │   ├── HomePage.tsx
│       │   ├── LoginPage.tsx
│       │   ├── NotFound.tsx
│       │   ├── PasswordRecoveryPage.tsx
│       │   └── SignupPage.tsx
│       ├── store/
│       └── utils/
└── server/
    ├── package.json
    └── src/
        ├── app.js
        ├── constants.js
        ├── index.js
        ├── controllers/
        │   ├── healthcheck.controller.js
        │   └── user.controller.js
        ├── db/
        │   └── index.js
        ├── middlewares/
        │   ├── auth.middleware.js
        │   └── multer.middleware.js
        ├── models/
        │   └── user.model.js
        ├── routes/
        │   ├── healthcheck.routes.js
        │   └── user.routes.js
        └── utils/
            ├── ApiError.js
            ├── ApiResponse.js
            ├── asyncHandler.js
            ├── cloudinary.js
            ├── collectionOwnerVerification.js
            ├── fetchMetadata.js
            ├── getPublicId.js
            └── sendMail.js
```

## Getting Started

### **Prerequisites**
- Node.js installed.
- MongoDB instance set up.

### **Installation**

1. Clone the repository:
   ```bash
   git clone https://github.com/Dhvanitmonpara/mern-starter-template.git
   ```

2. Navigate to the project directory:
   ```bash
   cd mern-starter-template
   ```

3. Install dependencies for both frontend and backend:
   ```bash
   cd ./client && npm install
   cd ./server && npm install
   ```

4. Set up environment variables:
   - Create a `.env` file in the `server/` and `client/` directories and add the respective variables.

### **Running the App**

1. Start the backend server:
   ```bash
   cd server && npm run dev
   ```

2. Start the frontend server:
   ```bash
   cd client && npm run dev
   ```

3. Open your browser and navigate to:
   - Frontend: `http://localhost:5173`
   - Backend: `http://localhost:8000`

## Scripts

### **Frontend**
- `npm run dev`: Start the React development server.
- `npm build`: Build the React app for production.

### **Backend**
- `npm run dev`: Start the backend server in development mode.
- `npm run build`: Build the backend for production.

## Tech Stack
- **Frontend**:
  - React (with React Router, Zustand, React Hook Form)
  - Tailwind CSS and ShadCN
  - TypeScript
  - Axios, React Icons
- **Backend**:
  - Node.js and Express.js
  - MongoDB with Mongoose
  - Socket.io
  - Nodemailer, Cloudinary

## Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

