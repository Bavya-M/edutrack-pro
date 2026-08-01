# EduTrack Pro — Smart Student Management System

A production-grade, portfolio-ready Student Management System built with React 19, Vite, Ant Design, and modern web technologies.

EduTrack Pro is a comprehensive academic management platform designed to streamline student administration, course management, attendance tracking, examination management, and performance analytics through an intuitive, responsive, and enterprise-inspired interface.

---

## ✨ Features

### 🔐 Authentication & Authorization

* **Secure JWT Authentication**
* **Role-Based Access Control** (Admin, Faculty, Student)
* **Password Encryption** using `bcrypt`
* **Protected Routes** & Session Management

### 👨‍🎓 Student Management

* Add, Update, Delete Students
* Search, Filter, and Pagination Support
* Student Profile Management & Photo Upload

### 👨‍🏫 Faculty Management

* Manage Faculty Records & Profiles
* Course Assignment & Department Allocation

### 📚 Course Management

* Create and Update Courses
* Assign Faculty & Manage Student Enrollment
* Department-wise Course Organization

### 🗓 Attendance Management

* Daily Attendance & Monthly Summaries
* Attendance Reports & Automatic Percentage Calculation

### 📊 Grade Management

* Marks Entry & Semester Results
* GPA Calculation & Academic Performance Tracking

### 📈 Dashboard & Analytics

* Student Statistics, Faculty Overview & Course Summaries
* Attendance Analytics & Grade Distribution Charts
* Recent Activity Feed

### 📄 Reports & UX

* Export reports to **PDF** and **Excel**
* Responsive Layout with **Dark / Light Mode**
* WCAG-friendly accessibility (ARIA labels, keyboard navigation, semantic HTML)

---

## 🛠 Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Frontend** | React 19, Vite, JavaScript (ES6+), React Router, Axios |
| **Backend** | Node.js, Express.js |
| **Database** | MongoDB, Mongoose |
| **UI Library** | Ant Design, Ant Design Icons, CSS Modules |
| **Authentication** | JSON Web Tokens (JWT), bcrypt |
| **Tooling** | ESLint, Prettier, Git, GitHub |
| **Deployment** | Vercel (Frontend), Render / Railway (Backend), MongoDB Atlas |

---

## 📂 Project Structure

```text
EduTrack-Pro/
│
├── client/                 # React Frontend
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── layouts/
│   │   ├── services/
│   │   ├── hooks/
│   │   ├── utils/
│   │   ├── context/
│   │   ├── routes/
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
│
├── server/                 # Node.js + Express Backend
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── utils/
│   ├── server.js
│   └── package.json
│
├── documentation/
├── .env.example
├── README.md
└── package.json

⚙️ Installation & Setup

1.Clone the repository:

git clone
 [https://github.com/Bavya-M/EduTrack-Pro.git](https://github.com/Bavya-M/EduTrack-Pro.git)

2.Install dependencies:

# Install server dependencies
cd server
npm install

# Install client dependencies
cd ../client
npm install

3.Configure Environment Variables:

PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
CLIENT_URL=http://localhost:5173

4.Run the Application:

# Terminal 1: Start Backend
cd server
npm run dev

# Terminal 2: Start Frontend
cd client
npm run dev

👥 User Roles & PermissionsRolePermissionsAdminFull system access, system-wide settings, user managementFacultyManage daily attendance, enter student grades, view assigned coursesStudentView personal profile, attendance statistics, and semester results
cd EduTrack-Pro

results🔗 REST API EndpointsMethodEndpointDescriptionAccessPOST/api/auth/loginUser LoginPublicPOST/api/auth/registerRegister UserPublic / AdminGET/api/studentsFetch list of studentsAdmin / FacultyPOST/api/studentsAdd a new studentAdminPUT/api/students/:idUpdate student profileAdminDELETE/api/students/:idRemove a studentAdminGET/api/coursesGet all coursesAuthenticatedPOST/api/attendanceRecord student attendanceFaculty / AdminPOST/api/gradesSubmit student gradesFaculty / Admin

🗄 Database Schema

Users: Stores authentication credentials, passwords (hashed), and global user roles.

Students: Contains profile data, registration details, and department linkage.

Faculty: Stores faculty credentials, assigned courses, and department allocations.

Courses: Contains course details, syllabi, faculty assignments, and enrolled students.

Attendance: Daily time-stamped attendance entries per student/course.

Grades: Academic evaluation marks, GPAs, and report metrics.

Departments: Academic department structures and metadata.

Notifications: System-wide alerts and updates.

🔒 Security Measures

JWT Authentication for stateless session management

Password Hashing with bcrypt

Role-Based Authorization (RBAC) middleware

Protected API Routes preventing unauthorized endpoints access

Input Validation on client and server sides

Environment Configuration handling sensitive keys securely

🤝 Contributing

Fork the repository.

Create a feature branch (git checkout -b feature/AmazingFeature).

Commit your changes (git commit -m 'Add some AmazingFeature').

Push to the branch (git push origin feature/AmazingFeature).

Open a Pull Request.

📄 License

This project is licensed under the MIT License.

👨‍💻 Author

Bavya M

BE - Computer Science and Engineering

A modern full-stack web application for managing student records, attendance, courses, grades, and user roles through a secure and intuitive dashboard.
