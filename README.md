

# Recipe Sharing Platform App with React & ExpressJS (MERN)

This project is a full-stack recipe sharing platform where users can view, save, and share recipes. The application is built using **React** for the frontend and **ExpressJS** with **Node.js** for the backend. The database is powered by **MongoDB** to store recipe data and user information.

## Features

- **User Authentication**: Sign up, log in, and log out functionality.
- **Recipe Management**: View, search, and save your favorite recipes.
- **Responsive Design**: The app works seamlessly on both desktop and mobile devices.
- **Real-time Data**: Fetch data from the backend and dynamically render recipes.

## Technologies Used

- **Frontend**: ReactJS, Axios, CSS (for styling)
- **Backend**: ExpressJS, Node.js
- **Database**: MongoDB
- **Authentication**: JWT (JSON Web Tokens) for secure login and authentication

## Installation & Setup

### 1. Clone the repository:

```bash
git clone https://github.com/yourusername/Recipe-Sharing-Platform-App-with-React-and-ExpressJS-Framework-MERN.git
cd Recipe-Sharing-Platform-App-with-React-and-ExpressJS-Framework-MERN
```

### 2. Set up the Backend (ExpressJS):

- Navigate to the `server` directory:

```bash
cd server
```

- Install dependencies:

```bash
npm install
```

- Create a `.env` file in the `server` directory and add your MongoDB URI and JWT secret:

```plaintext
MONGO_URI=<your-mongodb-uri>
JWT_SECRET=<your-jwt-secret>
```

- Start the backend server:

```bash
npm start
```

The backend will run on `http://localhost:5000` (by default).

### 3. Set up the Frontend (React):

- Navigate to the `client` directory:

```bash
cd client
```

- Install dependencies:

```bash
npm install
```

- Start the React app:

```bash
npm start
```

The frontend will run on `http://localhost:3000` (by default).

### 4. Open the application:

Once both the backend and frontend are running, you can open the app in your browser by visiting `http://localhost:3000`.

## Project Structure

```
Recipe-Sharing-Platform-App-with-React-and-ExpressJS-Framework-MERN/
│
├── client/                # React frontend
│   ├── public/            # Public assets (index.html, favicon, etc.)
│   └── src/               # Source code (components, hooks, pages, etc.)
│
├── server/                # Express backend
│   ├── models/            # Mongoose models (e.g., User, Recipe)
│   ├── routes/            # Express routes (API endpoints)
│   └── controllers/       # Route logic
│
├── .env                   # Environment variables (MongoDB URI, JWT secret)
├── package.json           # Backend dependencies
└── README.md              # Project documentation
```

## API Endpoints

### 1. **User Authentication**
- **POST** `/api/auth/signup` - Create a new user (requires `name`, `email`, `password`).
- **POST** `/api/auth/login` - Log in with `email` and `password`.

### 2. **Recipe Management**
- **GET** `/api/recipes` - Get all recipes.
- **GET** `/api/recipes/:id` - Get a single recipe by its `id`.
- **PUT** `/api/recipes/save` - Save a recipe to the user's account (requires `userID`, `recipeID`).
- **GET** `/api/recipes/savedRecipes/:userID` - Get saved recipes for a specific user.

## Contributing

We welcome contributions! Feel free to fork the repository and submit a pull request.

### Steps for Contribution:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature-name`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add feature'`)
5. Push to the branch (`git push origin feature/your-feature-name`)
6. Create a pull request

## License

This project is licensed under the MIT License.

## Acknowledgments

- [ReactJS](https://reactjs.org/) - JavaScript library for building user interfaces.
- [ExpressJS](https://expressjs.com/) - Fast, unopinionated web framework for Node.js.
- [MongoDB](https://www.mongodb.com/) - NoSQL database used for storing recipes and user data.
- [JWT](https://jwt.io/) - For secure authentication and authorization.

---
