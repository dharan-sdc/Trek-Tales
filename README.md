# Travel Book Story (MERN Stack)

A Full Stack Travel Story App built with MongoDB, Express, React, and Node.js. This application enables users to sign up, log in, and share personal travel stories. Features include image uploads, date tagging, search functionality, filtering by date range, and pinning favorite stories.

## Features

### Backend
- **Secure Authentication**: User authentication with JWT to ensure data privacy and security.
- **CRUD Operations**: APIs for creating, reading, updating, and deleting travel stories.
- **Image Upload**: Support for uploading and managing images (e.g., AWS S3 integration).
- **Search & Filter**: Search stories by keywords and filter them by date range.
- **Pin Stories**: API to pin favorite stories to the top.
- **Data Storage**: MongoDB for storing user profiles and travel stories.

### Frontend
- **User-Friendly UI**: Built with React and styled for responsive design.
- **Story Management**: Create, view, edit, and delete travel stories easily.
- **Interactive Features**: Search, filter, and pin stories for a personalized experience.

## Tech Stack
- **Frontend**: React, React Router, Axios
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: JSON Web Tokens (JWT)
- **Cloud Storage**: AWS S3 (or alternative for image handling)

## Installation

### Prerequisites
- Node.js (v16 or later)
- MongoDB installed locally or access to a MongoDB Atlas cluster

### Steps
1. Clone the repository:
   git clone https://github.com/username/travel-story-app.git
   cd travel-story-app
2.Install dependencies for both frontend and backend:

    cd backend
    npm install
    
    cd ../frontend
    npm install

3.Configure environment variables:
Create a .env file in the backend directory and add the following:

    PORT=5000
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    CLOUD_STORAGE_KEY=your_cloud_storage_key (optional)
    Start the development servers:

**Backend:**
cd backend
npm start

**Frontend:**
cd frontend
npm run dev

Access the app at http://localhost:8000.

## Folder Structure
travel-story-app/
│
├── backend/
│   ├── controllers/      # API logic
│   ├── models/           # MongoDB schemas
│   ├── routes/           # API endpoints
│   ├── middleware/       # Authentication & error handling
│   └── server.js         # Entry point
│
├── frontend/
│   ├── src/
│   │   ├── components/   # React components
│   │   ├── pages/        # App pages
│   │   ├── hooks/        # Custom React hooks
│   │   └── App.js        # Main React app
│
└── readme.md             # Project documentation


## API Endpoints
**User Routes**
- POST /api/users/register - Register a new user
- POST /api/users/login - Log in a user
- GET /api/users/profile - Fetch user profile (requires authentication)

**Story Routes**
- GET /api/stories - Fetch all stories
- POST /api/stories - Create a new story
- PUT /api/stories/:id - Update a story
- DELETE /api/stories/:id - Delete a story
- GET /api/stories/search - Search and filter stories

## Contributing
Fork the project.
Create a feature branch:

git checkout -b feature/YourFeature
Commit your changes:

git commit -m "Add your feature"
Push to the branch:

git push origin feature/YourFeature
Open a pull request.

## License
This project is licensed under the MIT License.
