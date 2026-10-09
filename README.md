Wanderlust

A travel listing platform where users can explore, list and review travel destinations. Built with Node.js, Express and MongoDB.

## Features

- User authentication and authorization
- CRUD operations for travel listings
- Image upload with Cloudinary
- Interactive maps with Mapbox
- User reviews and ratings
- Category-based filtering
- Search functionality
- Responsive design

## Tech Stack

- **Frontend**: EJS, Bootstrap, CSS
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Authentication**: Passport.js
- **Image Storage**: Cloudinary
- **Maps**: Mapbox
- **Additional Tools**:
  - Multer for file uploads
  - Express-session for session management
  - Connect-flash for flash messages
  - Method-override for HTTP methods
  - Mongoose for MongoDB object modelings

## Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/wanderlust.git
cd wanderlust
```

2. Install dependencies:

```bash
npm install
```

3. Create a `.env` file in the root directory with the following variables:

```
CLOUD_NAME=your_cloudinary_cloud_name
CLOUD_API_KEY=your_cloudinary_api_key
CLOUD_API_SECRET=your_cloudinary_api_secret
MAP_TOKEN=your_mapbox_token
ATLASTDB_URL=your_mongodb_url
SECRET=your_session_secret
```

4. Start the server:

```bash
node app.js
```

The application will be available at `http://localhost:8080`

## Project Structure

```
├── controllers/        # Route controllers
├── models/            # Database models
├── routes/            # Route definitions
├── views/
│   ├── includes/      # Reusable EJS components
│   ├── layouts/       # Page layouts
│   ├── listings/      # Listing views
│   └── users/         # User-related views
├── public/
│   ├── css/          # Stylesheets
│   └── js/           # Client-side JavaScript
├── utils/            # Utility functions
├── middleware.js     # Custom middleware
├── app.js           # Main application file
└── package.json
```

## Features in Detail

### Listings

- Create, read, update and delete travel listings
- Upload and manage listing images
- Location mapping with Mapbox integration
- Category-based filtering
- Search by location

### User Management

- User registration and authentication
- Profile management
- Authorization for listing operations

### Reviews

- Add and delete reviews
- Star rating system
- Review author verification
