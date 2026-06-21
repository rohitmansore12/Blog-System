# Blog System

A full-stack Blog Management System built with **Node.js, Express.js, MySQL, EJS, and Bootstrap**. The platform allows users to create, edit, and manage blog posts, while administrators can moderate and approve content through a dedicated admin dashboard.

## Overview

Blog System is a content management platform featuring secure authentication, role-based access control, image uploads, post approval workflow, and a responsive user interface.

---

## Features

### User Features

* User Registration & Login
* Secure Password Hashing (bcryptjs)
* Session-Based Authentication
* Create, Read, Update & Delete Blog Posts
* Rich Text Editor for Content Writing
* Image Upload Support
* Personal Dashboard
* User Profile Management
* Pagination Support

### Admin Features

* Admin Dashboard
* User Management
* View All Posts
* Post Approval System
* Content Moderation

### General Features

* Responsive Design using Bootstrap 5
* Flash Messages for User Feedback
* Role-Based Access Control
* MySQL Database Integration

---

## Tech Stack

### Frontend

* HTML5
* CSS3
* JavaScript (ES6+)
* Bootstrap 5
* EJS
* Font Awesome

### Backend

* Node.js
* Express.js
* Express Session
* bcryptjs
* Multer

### Database

* MySQL

### Additional Packages

* express-validator
* connect-flash
* sanitize-html

---

## Project Structure

```text
Blog-System/
│
├── controllers/
│   ├── indexController.js
│   ├── userController.js
│   ├── postController.js
│   └── adminController.js
│
├── routes/
│   ├── index.js
│   ├── users.js
│   ├── posts.js
│   └── admin.js
│
├── views/
├── public/
│   ├── uploads/
│   ├── images/
│   └── richtexteditor/
│
├── db.js
├── index.js
├── package.json
└── README.md
```

---

## Installation

### Prerequisites

* Node.js
* npm
* MySQL Server

### Clone Repository

```bash
git clone https://github.com/rohitmansore12/Blog-System.git
cd Blog-System
```

### Install Dependencies

```bash
npm install
```

### Database Setup

Create a MySQL database:

```sql
CREATE DATABASE blog;
```

Import the provided `blog.sql` file into MySQL.

### Configure Database

Update database credentials inside `db.js`:

```javascript
const db = mysql.createConnection({
  host: "localhost",
  user: "root",
  password: "",
  database: "blog"
});
```

### Run Application

```bash
npm start
```

For development:

```bash
npm run dev
```

Open in browser:

```text
http://localhost:5000
```

---

## Usage

### Regular User

1. Register a new account
2. Login with your credentials
3. Create blog posts
4. Upload images
5. Edit or delete your posts
6. Manage content through dashboard

### Administrator

1. Login as Admin
2. Access Admin Dashboard
3. Manage Users
4. Review Posts
5. Approve Posts

---

## Security Features

* Password Hashing using bcryptjs
* Session-Based Authentication
* SQL Injection Prevention using Parameterized Queries
* File Upload Validation
* Input Validation
* Role-Based Authorization

---

## Future Improvements

* Search Functionality
* Categories & Tags
* Comments System
* Password Reset
* Email Verification
* Dark Mode
* Notifications
* Like & Bookmark Feature

---

## Author

**Rohit Mansore**

GitHub: https://github.com/rohitmansore12

⭐ If you found this project useful, consider giving it a star.


