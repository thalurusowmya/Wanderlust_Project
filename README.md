
# WanderLust - Travel & Accommodation Platform

check website : https://wanderlust2-ctql.onrender.com/listings

WanderLust is a full-stack web application built with Node.js, Express, and MongoDB that allows users to explore, list, and review travel accommodations.

## 🌟 Features

### User Authentication & Authorization
- Secure user registration and login system
- Password encryption using Passport.js
- Session management with MongoDB store
- User-specific access control for listings and reviews

### Listings Management
- Create, read, update, and delete (CRUD) operations for property listings
- Detailed property information including:
  - Title and description
  - Price
  - Location and country
  - Images (with cloud storage support)
- Search and filter capabilities

### Review System
- Users can leave reviews for listings
- Review validation and moderation
- Review management (create/delete)
- Author-only review deletion

### Security Features
- Protected routes using middleware
- Input validation and sanitization
- Flash messages for user feedback
- Error handling middleware
- Secure session management

### Technical Stack
- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: Passport.js
- **Template Engine**: EJS
- **Styling**: Custom CSS
- **File Storage**: Cloud storage integration
- **Session Management**: Express-session with MongoDB store

## 🚀 Getting Started

### Prerequisites
- Node.js
- MongoDB
- npm or yarn

### Installation
1. Clone the repository
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file with the following variables:
   ```
   ATLASDB_URL=your_mongodb_connection_string
   SECRET=your_session_secret
   ```
4. Start the server:
   ```bash
   node app.js
   ```

## 🔧 Environment Variables
- `ATLASDB_URL`: MongoDB connection string
- `SECRET`: Session secret key
- `NODE_ENV`: Environment (development/production)

## 📁 Project Structure
```
├── controllers/     # Route controllers
├── models/         # Database models
├── routes/         # Express routes
├── views/          # EJS templates
├── public/         # Static files
├── utils/          # Utility functions
├── middleware.js   # Custom middleware
├── app.js          # Main application file
└── package.json    # Project dependencies
```

## 🔐 Security Features
- Password hashing
- Session-based authentication
- Protected routes
- Input validation
- XSS protection
- CSRF protection

## 🛠️ API Endpoints
- `/listings` - Listing management
- `/listings/:id/reviews` - Review management
- `/` - User authentication routes

