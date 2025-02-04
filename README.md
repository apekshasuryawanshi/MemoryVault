# Sylora

Sylora is the ultimate destination for travel enthusiasts, Its modern blog offers inspiring stories, expert tips and insider guides to explore the whole world. Built with cutting-edge web technologies, Sylora aims to provide a seamless, user-friendly interface for its users.

## Features

### Core Features
* **User Management**
  * Secure user authentication and account creation
  * Personalized user profiles
  * Role-based access for contributors and viewers

* **Content Management**
  * User-friendly interface for content creation and editing
  * Integration of multimedia elements like images and videos
  * Categorization and tagging for easy navigation

* **Engagement Tools**
  * Commenting and feedback system
  * Content sharing capabilities across social media
  * Notifications for updates and activities


## Technology Stack

### Frontend
* React.js
* Tailwind CSS for modern, responsive design
* React Router for navigation
* Axios for HTTP requests

### Backend
* Node.js
* Express.js
* MongoDB with Mongoose for database management
* JWT for secure authentication

### Deployment
* Cloud hosting on Render/Vercel

## Getting Started

### Prerequisites
* Node.js installed on your machine
* MongoDB installed locally or a MongoDB Atlas account
* Docker (optional for deployment)
* NPM or Yarn package manager


### Installation

1. Clone the repository
```bash
git clone https://github.com/himanshu-o5/sylora.git
cd sylora
```

2. Install dependencies for backend
```bash
cd api
npm install
```

3. Install dependencies for frontend
```bash
cd frontend
npm install
```

4. Create a `.env` file in the backend directory with the following variables:
```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
API_KEY=your_api_key
```

5. Start the backend server
```bash
cd backend
npm start
```

6. Start the frontend application
```bash
cd frontend
npm run dev
```

## Database Schema

### Stories Schema
```javascript
{
  title: {type: String, required: true},
    story: {type: String, required: true},
    visitedLocation: {type: [String], default: []},
    isFavourite: {type: Boolean, default: false},
    userId: {type: Schema.Types.ObjectId, ref: "User", required: true},
    createdOn: {type: Date, default: Date.now},
    imageUrl: {type: String, required: true},
    visitedDate: {type: Date, required: true},
}
```

### UserSchema
```javascript
{
  fullName: String,
  email: String,
  password: String,
  createdOn: Number
}
```





## Security Features
* Password encryption with bcrypt
* Role-based access control
* JWT Tokens
* Protected API endpoints

## Contributing
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments
* MongoDB Documentation
* Express.js Documentation
* React.js Documentation
* Node.js Documentation
* Razorpay Documentation