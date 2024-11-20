
# EntryWay

EntryWay is a comprehensive web application designed to facilitate the exploration and booking of monuments. It offers users detailed information about various monuments and enables seamless booking experiences.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Monument Exploration**: Browse and search for monuments with detailed information.
- **Booking System**: Securely book visits to monuments.
- **Admin Panel**: Manage monuments, bookings, and user information.
- **User Authentication**: Secure login and registration system.
- **Responsive Design**: Optimized for various devices and screen sizes.

## Technologies Used

- **Frontend**:
  - React.js
  - React Router
  - Axios
  - CSS Modules

- **Backend**:
  - Node.js
  - Express.js
  - MongoDB
  - Mongoose
  - JWT for authentication

- **Deployment**:
  - Vercel for frontend
  - Render for backend

## Installation

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- MongoDB instance

### Backend Setup

1. **Clone the repository**:

   ```bash
   git clone https://github.com/slvarun/EntryWay.git
   cd EntryWay/EntryWayBackEnd
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Set up environment variables**:

   Create a `.env` file in the root directory with the following content:

   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   ```

4. **Start the backend server**:

   ```bash
   npm start
   ```

   The server will run on `http://localhost:5000`.

### Frontend Setup

1. **Navigate to the frontend directory**:

   ```bash
   cd ../EntryWayFrontEnd
   ```

2. **Install dependencies**:

   ```bash
   npm install
   ```

3. **Set up environment variables**:

   Create a `.env` file in the root directory with the following content:

   ```env
   REACT_APP_API_URL=http://localhost:5000
   ```

4. **Start the frontend application**:

   ```bash
   npm start
   ```

   The application will run on `http://localhost:3000`.

## Usage

1. **Access the application**:

   Open your browser and navigate to `http://localhost:3000`.

2. **Explore Monuments**:

   Browse through the list of monuments, view details, and make bookings.

3. **Admin Panel**:

   Access the admin panel to manage monuments, bookings, and users.

## Project Structure

```
EntryWay/
├── EntryWayBackEnd/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── .env
│   ├── app.js
│   └── package.json
└── EntryWayFrontEnd/
    ├── public/
    ├── src/
    │   ├── components/
    │   ├── pages/
    │   ├── App.js
    │   └── index.js
    ├── .env
    └── package.json
```

## API Endpoints

### Authentication

- **Register**: `POST /auth/register`
- **Login**: `POST /auth/login`

### Monuments

- **Get All Monuments**: `GET /monuments`
- **Get Monument by ID**: `GET /monuments/:id`
- **Create Monument**: `POST /monuments` (Admin only)
- **Update Monument**: `PUT /monuments/:id` (Admin only)
- **Delete Monument**: `DELETE /monuments/:id` (Admin only)

### Bookings

- **Create Booking**: `POST /bookings`
- **Get Booking by ID**: `GET /bookings/:id`
- **Get All Bookings**: `GET /bookings` (Admin only)

## Contributing

Contributions are welcome! Please follow these steps:

1. **Fork the repository**.
2. **Create a new branch**:

   ```bash
   git checkout -b feature/your-feature-name
   ```

3. **Make your changes**.
4. **Commit your changes**:

   ```bash
   git commit -m "Add your commit message"
   ```

5. **Push to your branch**:

   ```bash
   git push origin feature/your-feature-name
   ```

6. **Create a Pull Request**.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details. 
