# Full Stack Project

## Project Overview
This is a Full Stack educational management system that supports two types of users: **Teachers** and **Students**. The application allows teachers to manage classes, students, homework, and grades. Students can view their grades and submit homework assignments.

### Team Members:
- **Laith Khater** (ID: 323965152)
- **Rami Hanna** (ID: 323956557)

---

## Features

### User Types:
1. **Teacher**:
    - Add new classes and assign grades.
    - Add students to classes.
    - Assign homework with due dates and file uploads.
    - Track and update attendance.
    - Edit grades.
    - View class performance and visualize grades using charts.

2. **Student**:
    - View grades for all courses, including the final grade.
    - Submit homework assignments through the portal.

### General Features:
- **Authentication**: Secure login and registration for both teachers and students.
- **Logging**: Logging of exceptions and user actions.
- **Graphical Representation**: Teachers can view grade distributions using charts.
- **Responsive Design**: The application is fully responsive and user-friendly.

---

## Technology Stack

### Frontend:
- **HTML**
- **CSS**
- **JavaScript**
- **Bootstrap**

### Backend:
- **Node.js**
- **Express.js**

### Database:
- **phpMyAdmin** (SQL Server)

### Additional Libraries & Tools:
- **React.js**
- **axios**
- **Chart.js**
- **React-Toastify**
- **bcrypt** (For password encryption)
- **jsonwebtoken** (For user authentication)
- **multer** (For file uploads)
- **mysql** (Database integration)

---

## Installation Instructions

### Prerequisites:
- Node.js and npm installed on your system.
- MySQL or phpMyAdmin installed for the database.

### Steps to Install:
1. **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/full-stack-project.git
    ```
2. **Navigate to the project directory:**
    ```bash
    cd full-stack-project
    ```
3. **Install dependencies:**
    ```bash
    npm install
    ```
4. **Setup the database:**
    - Import the provided SQL file into your MySQL database.
    - Update the `config/db.js` file with your database credentials.

5. **Run the application:**
    ```bash
    npm start
    ```

6. **Access the app**:
    Open your browser and navigate to `http://localhost:3000`.

---

## API Documentation

The project provides a RESTful API for performing various actions.

### Endpoints:

1. **Register**: `/register`
    - **Method**: POST
    - **Description**: Register a new user (Teacher or Student).
    - **Request**: 
      ```json
      {
        "fname": "John",
        "lname": "Doe",
        "email": "john.doe@example.com",
        "phone": "123-456-7890",
        "password": "securepassword123",
        "role": "Student"
      }
      ```
    - **Response**:
      ```json
      {
        "Message": "Student registered successfully!"
      }
      ```

2. **Login**: `/login`
    - **Method**: GET
    - **Request**: Query Parameters for `email` and `password`
    - **Response** (Teacher):
      ```json
      {
        "success": true,
        "message": "Login successful",
        "role": "Teacher"
      }
      ```

(Include other endpoints as needed from your project.)

---

## Database Schema

- **students**: Stores student details.
- **teachers**: Stores teacher details.
- **classes**: Stores class information.
- **tasks**: Stores homework tasks assigned to classes.
- **attendance**: Tracks attendance for students in classes.

---

## Screenshots

### Home Page:
![Home Page](link-to-image)

### Teacher Dashboard:
![Teacher Dashboard](link-to-image)

### Student Grades Page:
![Student Grades](link-to-image)

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Contact

For any inquiries, please reach out to:
- **Rami Hanna**: [LinkedIn](https://www.linkedin.com/in/ramihanna17) | [GitHub](https://github.com/RamiHann)
- **Laith Khater**: [Contact Info]

```

### Instructions:
1. Replace placeholders like `your-username` and `link-to-image` with actual values.
2. Add or remove sections as needed for your project.
3. If you don't have screenshots yet, you can generate them and upload them later to GitHub.

Feel free to adjust the API documentation, installation steps, or other sections to suit your project requirements!