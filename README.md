# Travel Book Story (MERN Stack)

A Full Stack Travel Story App built with MongoDB, Express, React, and Node.js. This application enables users to sign up, log in, and share personal travel stories. Features include image uploads, date tagging, search functionality, filtering by date range, and pinning favorite stories.

---

## Live Demo
This project is live! Explore it here: [Travel Book Journey App - Trek Tales](https://trektales.vercel.app/login)

------

## Demo

### 1. Login Page
![Login Page Demo](https://github.com/user-attachments/assets/ea70dce7-610a-4b90-b68a-5fbf4b41883b)

### 2. Dashboard
The dashboard allows users to view their profile and access all features.
![Dashboard Demo](https://github.com/user-attachments/assets/b7077ef5-6a03-4b14-bbc3-439f19a336ac)


### 3. Create a New Story
Users can create a new travel story, upload images, and add tags.
![Create Story Demo](https://github.com/user-attachments/assets/bcf8e012-b9c4-4456-911b-f95ba5b6f60d)


### 4. View and Update Stories
View all posted stories, update them, or delete as needed.
![Story View Demo](https://github.com/user-attachments/assets/5b9789d5-4939-4de1-8bc2-619ea1e26cb7)

### 5. Filter by date
Intuitive date range filters to refine story search.
![Filter date range](https://github.com/user-attachments/assets/4e33b8a3-89cf-4cb1-886b-1e558c5b4c28)


### 6. Mobile View
Responsive design optimized for mobile devices.
![Mobile View](https://github.com/user-attachments/assets/1e7f6412-76b6-44d7-b74d-e51fba9e4fca)


---
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

   
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret

**Backend:**
cd backend
npm install

**Frontend:**
cd ../frontend
npm install

Access the app at http://localhost:8000.

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
