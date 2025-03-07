# Fitness Tracker Application

The Fitness Tracker Application is a full-stack web application built with Spring Boot (backend) and React (frontend). It allows users to track their fitness goals, log calories burned, and calculate their BMI. The application provides a seamless user experience with features like goal tracking, progress visualization, and user authentication.

## Features

### User Authentication
- Users can register, log in, and log out.
- Protected routes ensure only authenticated users can access the dashboard.

### Goal Tracking
- Users can create, update, and delete fitness goals.
- Goals can be marked as "Completed" or "Not Completed."
- A progress bar shows the percentage of completed goals.

### Calorie Tracking
- Users can log calories burned for each goal.
- The total calories burned are displayed on the dashboard.

### BMI Calculator
- Users can calculate their BMI by entering their weight and height.
- The BMI result is displayed along with standard BMI categories.

### Visualization
- A pie chart shows the progress of completed vs. remaining goals.
- The total calories burned are displayed as a text value.

### Responsive Design
- The application is fully responsive and works on all devices.

## Technologies Used

### Backend
- **Spring Boot**: Java framework for building the REST API.
- **Spring Data JPA**: For database interaction.
- **MySQL**: Relational database for storing user and goal data.
- **Spring Security**: For user authentication and authorization (optional).

### Frontend
- **React**: JavaScript library for building the user interface.
- **React Router**: For client-side routing.
- **Axios**: For making HTTP requests to the backend.
- **Bootstrap**: For styling and responsive design.
- **Chart.js**: For visualizing data (pie chart).

## Setup Instructions

### 1. Prerequisites
- **Java Development Kit (JDK)**: Version 17 or higher.
- **Node.js**: Version 16 or higher.
- **MySQL**: Installed and running locally or remotely.
- **Maven**: For building the Spring Boot project.

### 2. Backend Setup
#### Clone the repository:
```bash
git clone https://github.com/your-username/fitness-tracker.git
cd fitness-tracker/backend
```

#### Configure the database:
Update the `application.properties` file with your MySQL credentials:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/fitness_tracker
spring.datasource.username=your-username
spring.datasource.password=your-password
spring.jpa.hibernate.ddl-auto=update
```

#### Run the Spring Boot application:
```bash
mvn spring-boot:run
```
The backend will start at `http://localhost:8080`.

### 3. Frontend Setup
#### Navigate to the frontend directory:
```bash
cd ../frontend
```

#### Install dependencies:
```bash
npm install
```

#### Start the React development server:
```bash
npm start
```
The frontend will start at `http://localhost:5173`.

## API Endpoints

### User Authentication
- **POST** `/api/users/register`: Register a new user.
- **POST** `/api/users/login`: Log in an existing user.

### Goals
- **GET** `/api/goals/user/{userId}`: Get all goals for a user.
- **POST** `/api/goals`: Create a new goal.
- **PUT** `/api/goals/{id}`: Update a goal.
- **DELETE** `/api/goals/{id}`: Delete a goal.
- **DELETE** `/api/goals/user/{userId}`: Delete all goals for a user.

### BMI Calculator
- **POST** `/api/bmi/calculate`: Calculate BMI.
- 
## Acknowledgments
- **Spring Boot**: For providing a robust backend framework.
- **React**: For enabling a dynamic and responsive frontend.
- **Bootstrap**: For making the UI design process easier.
- **Chart.js**: For data visualization.


Thank you for checking out the Fitness Tracker Application! 🚀

