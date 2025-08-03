Game Development Training Center Website
This project is a full-stack, responsive website for a Game Development Training Center, built to showcase a range of development skills. It features a user-friendly frontend for course information and registration, backed by a robust API.

The website is designed with a striking dark, shiny purple and black color scheme, offering a modern and engaging user experience.

🚀 Features
Home Page: An inviting introduction to the center, a prominent call-to-action banner, and an overview of what the center offers.

Courses Page: A detailed list of available courses (e.g., Unity, Unreal Engine, Game Design, 2D/3D Art), each with a title, image, brief description, and duration.

Registration Page: A form for students to register, including fields for Full Name, Email, Phone Number, Course Selection, and a Message, with basic client-side validation.

About Us Page: Information about the center's mission, expert team, and overarching goals.

Contact Page: Provides contact details (address, email, phone) and an embedded Google Map, along with a contact form.

Admin Panel (Bonus): A basic dashboard to view all registered students, demonstrating backend data retrieval.

🛠️ Tech Stack
This project utilizes a modern MERN (MongoDB, Express, React, Node.js) stack:

Frontend:

React: Built with Create React App (CRA) for a robust and scalable single-page application.

React Router DOM: For seamless navigation between pages.

Bootstrap: Used for responsive design and UI components.

Material-UI (MUI): Provides a rich set of React components and icons for enhanced aesthetics and functionality.

Axios: For making HTTP requests to the backend API.

Backend:

Node.js: JavaScript runtime environment.

Express.js: A fast, unopinionated, minimalist web framework for Node.js.

Mongoose: ODM (Object Data Modeling) library for MongoDB and Node.js.

Dotenv: For managing environment variables.

CORS: Middleware to enable Cross-Origin Resource Sharing.

Database:

MongoDB: A NoSQL document database for flexible data storage.

⚙️ Setup and Installation
Follow these steps to get the project up and running on your local machine.

Prerequisites
Before you begin, ensure you have the following installed:

Node.js (v14 or higher) & npm (Node Package Manager)

MongoDB Atlas account (recommended for cloud database) or a local MongoDB instance running.

1. Backend Setup (server directory)
Navigate to the server directory in your terminal:

cd server

Install backend dependencies:

npm install

Create a .env file in the server directory. This file will store your sensitive environment variables.

# On Windows
echo > .env
# On macOS/Linux
touch .env

Add your MongoDB connection string and desired port to the .env file. Remember to replace <db_password> with your actual MongoDB password.

PORT=5000
MONGODB_URI="mongodb+srv://sivasuthansaranyasarma1:<db_password>@cluster0.zonyzm5.mongodb.net/game_dev_center_db?retryWrites=true&w=majority&appName=Cluster0"

(Ensure your MongoDB user has the necessary permissions and network access configured in MongoDB Atlas.)

Start the backend server:

npm run dev

You should see a message indicating that the server is running on port 5000 and MongoDB is connected.

2. Frontend Setup (client directory)
Navigate back to the root project directory (game-dev-center), then go into the client directory:

cd ../client

Install frontend dependencies:

npm install

Create the assets folder inside client/src and place your course images (unity.jpg, unreal.jpg, gamedesign.jpg, art.jpg) there. You can use placeholder images if you don't have specific ones ready.

mkdir src/assets
# Then manually copy your images into src/assets

Start the frontend development server:

npm start

The React application will open in your browser, typically at http://localhost:3000.

🌐 Usage
Once both the backend and frontend servers are running, open your web browser and navigate to http://localhost:3000.

Explore the different pages using the navigation bar.

Test the registration form on the "Registration" page. Submissions will be stored in your MongoDB database.

(Bonus) Access the admin panel by navigating to http://localhost:3000/admin to view registered students.

🤝 Contributing
Feel free to fork this repository, make improvements, and submit pull requests.

📄 License
This project is open-source and available under the MIT License.
