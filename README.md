# Request Management System

This repository contains a **Request Management System** built using the **MERN stack** (MongoDB, Express, React, Node.js) with **TypeScript**. The system allows users to manage requests efficiently by performing CRUD operations (Create, Read, Update, Delete) and features a responsive design with functional components such as a navigation bar, status circles, and request table.

The goal of this project is to demonstrate a complete full-stack application with a focus on user experience, responsiveness, and adherence to TypeScript best practices.

## Objective
The objective of this project is to develop a Request Management System that allows users to:
- View requests in a table with filtering options.
- Add new requests through a form.
- Edit or delete requests.
- Monitor the status of requests using responsive UI components such as circles.

## Features
- **Responsive Design**: The application adapts to various screen sizes, ensuring usability on mobile and desktop devices.
- **CRUD Operations**:
  - **GET**: Retrieve the list of requests.
  - **POST**: Add new requests.
  - **PATCH**: Update existing requests.
  - **DELETE**: Remove requests.
- **TypeScript**: The project utilizes TypeScript throughout both the frontend and backend to ensure strong typing and improved code quality.
- **Responsive Navbar**: Highlights active sections (Dashboard, Requests, Feedbacks, Reports, Patient, Settings), with a dropdown in the Settings section.
- **Request Status Circles**: Visual representation of request statuses such as New, In Progress, Escalated, and On Hold.
- **Mobile Responsive Request Table**: A table with status and priority badges, including filters for status and department.
- **Form for Adding/Editing Requests**: A form with fields such as Request ID, Status, Priority, Department, etc.
- **API Endpoints**: Defined to handle CRUD operations with validation and error handling.

## Project Structure
The project follows an atomic design structure and modular approach with separate directories for the frontend and backend.

- **Frontend (React with TypeScript)**:
  - **Navbar**: Displays active states and includes a dropdown for the settings section.
  - **Status Circles**: Displays the count of requests in different statuses.
  - **Request Table**: Shows a list of requests with filters and mobile responsiveness.
  - **Form**: Used to add or edit requests, with form validation.
  - **Modals**: Used for editing and deleting requests.

- **Backend (Node.js with Express & MongoDB)**:
  - **API Endpoints**:
    - `GET /requests`: Fetch all requests.
    - `POST /requests`: Add a new request.
    - `PATCH /requests/:id`: Update a request.
    - `DELETE /requests/:id`: Delete a request.

## Setup Instructions

### Prerequisites
To set up this project, you need the following installed on your system:
- **Node.js** (v14 or higher)
- **MongoDB** (For local development or connect to a cloud database)
- **TypeScript** (Globally installed)
- **Git**

### Installation Steps

1. **Clone the repository**:
   git clone https://github.com/DisuC/Request-Management-System |
   cd request-management-system

2. **Install Dependencies**:
   - For **Frontend**:
     cd client |
     npm install

   - For **Backend**:
     cd server |
     npm install

3. **Environment Variables**:
   - In the `server` directory, create a `.env` file and add your MongoDB connection string:
     MONGO_URI=mongodb://localhost:27017/request-management

4. **Run the Development Servers**:
   - **Backend (Server)**:
     cd server |
     npm run dev
   
   - **Frontend (Client)**:
     cd client |
     npm start

5. **Access the Application**:
   - Open your browser and go to `http://localhost:3000` to view the frontend.
   - The API will be available at `http://localhost:5000`.

### Testing the API
You can test the API endpoints using **Postman** or similar tools:
- **GET /requests**: Retrieve all requests.
- **POST /requests**: Create a new request.
- **PATCH /requests/:id**: Update an existing request.
- **DELETE /requests/:id**: Delete a request.

## Bonus Features
- **Authentication and Authorization**
- **Unit and Integration Tests**
- **Cloud Deployment**: You can deploy the application using platforms like **Heroku**, **Vercel**, or **Netlify**.

## Technologies Used
- **Frontend**:
  - **React.js with TypeScript**
  - **HTML/CSS**
  - **Tailwind CSS** (optional for styling)
- **Backend**:
  - **Node.js with Express**
  - **MongoDB**
  - **Mongoose** (for MongoDB models)
- **API Testing**: Postman
- **Version Control**: Git & GitHub
