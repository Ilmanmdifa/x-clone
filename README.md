# Twitter Clone

A full-stack Twitter clone built with the MERN (MongoDB, Express, React, Node.js) stack. This application replicates core Twitter features such as posting, liking, commenting, following/unfollowing users, and notifications.

---

## Demo

To see the app in action, follow the [Installation](#installation) steps to run it locally on your machine.

## Features

- **Authentication**: Signup, login, and logout functionality with JWT-based authentication.
- **Posts**:
  - Create posts with text and optional images.
  - Like/unlike posts.
  - Comment on posts.
- **User Profiles**:
  - View user profiles with follower/following counts.
  - Edit profile details, including profile and cover images.
- **Follow System**:
  - Follow/unfollow users.
  - Suggested users to follow.
- **Notifications**:
  - Receive notifications for likes and follows.
  - Mark notifications as read or delete them.
- **Responsive Design**: Optimized for desktop and mobile devices.
- **Real-Time Updates**: React Query for efficient state management and data fetching.

---

## Installation

### Prerequisites
- Node.js (v16+)
- MongoDB (local or cloud instance)
- Cloudinary account (for image uploads)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/twitter-clone.git
   cd twitter-clone
2. Install dependencies for both the backend and frontend:
   ```bash   
    # Backend
    cd backend
    npm install
    
    # Frontend
    cd ../frontend
    npm install
3. Set up environment variables by creating a .env file in the backend folder with the following:
   ```bash
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
   CLOUDINARY_API_KEY=your_cloudinary_api_key
   CLOUDINARY_API_SECRET=your_cloudinary_api_secret
   PORT=5000
4. Start the development servers:
   ```bash
   # Backend
   cd backend
   npm run dev
    
   # Frontend
   cd ../frontend
   npm run dev
5. Open the app in your browser at http://localhost:3000.

## Usage
1. Signup/Login: Create an account or log in with an existing one.
2. Create Posts: Share text or images with your followers.
3. Follow Users: Follow other users to see their posts in your "Following" feed.
4. Like and Comment: Interact with posts by liking or commenting on them.
5. Edit Profile: Update your profile details, including profile and cover images.
6. Notifications: View notifications for likes and follows.

## Technologies Used
### Backend
- Node.js: JavaScript runtime for building the server.
- Express.js: Web framework for handling API routes.
- MongoDB: NoSQL database for storing user, post, and notification data.
- Mongoose: ODM for MongoDB.
- Cloudinary: Image hosting and management.
- JWT: Authentication using JSON Web Tokens.
### Frontend
- React: Frontend library for building the user interface.
- React Router: Client-side routing.
- React Query: State management and server-state synchronization.
- Tailwind CSS: Utility-first CSS framework for styling.
- DaisyUI: Tailwind CSS components for UI elements.

## Folder Structure
```bash
twitter-clone/
├── backend/
│   ├── controllers/       # API controllers for handling requests
│   ├── db/                # MongoDB connection setup
│   ├── lib/               # Utility functions
│   ├── middleware/        # Middleware (e.g., authentication)
│   ├── models/            # Mongoose models for MongoDB
│   ├── routes/            # API routes
│   └── [server.js](http://_vscodecontentref_/1)          # Entry point for the backend
├── frontend/
│   ├── public/            # Static assets
│   ├── src/
│   │   ├── components/    # Reusable React components
│   │   ├── hooks/         # Custom React hooks
│   │   ├── pages/         # Page components for routing
│   │   ├── utils/         # Utility functions
│   │   └── [main.jsx](http://_vscodecontentref_/2)       # Entry point for the frontend
│   ├── [index.html](http://_vscodecontentref_/3)         # HTML template
│   └── [vite.config.js](http://_vscodecontentref_/4)     # Vite configuration
├── .env                   # Environment variables (not included in the repo)
├── [package.json](http://_vscodecontentref_/5)           # Project metadata and dependencies
└── [README.md](http://_vscodecontentref_/6)              # Project documentation
