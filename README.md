# Student Progress Management System

A comprehensive Django-based web application for managing student information and tracking academic progress with exam results and performance analytics.

## Features

- **User Authentication**: Secure signup/login with OTP verification
- **Student Management**: CRUD operations for student records
- **Progress Tracking**: Exam-based progress sheets with multiple subjects
- **Filtering & Search**: Advanced filtering by exam type, class, and search functionality
- **Dashboard**: Admin dashboard with student statistics and navigation
- **Responsive Design**: Mobile-friendly interface with modern UI

## Technologies Used

- Python 3.7+
- Django 3.2+
- SQLite (default database)
- HTML5, CSS3, JavaScript
- Bootstrap 5
- Font Awesome

## Setup Instructions

### Prerequisites

- Python 3.7 or higher
- pip (Python package installer)

1. **Run database migrations**:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```


2. **Start the development server**:
   ```bash
   python manage.py runserver
   ```

3. **Access the application**:
   - Open your browser and go to `http://127.0.0.1:8000/`
   - The admin panel is available at `http://127.0.0.1:8000/admin/`

## Application Workflow

### For New Users:
1. Navigate to the signup page
2. Enter email and password (confirm password)
3. You'll be redirected to OTP verification (in this simplified version, just click verify)
4. After verification, you can log in

### For Admin Users:
1. Login with your credentials
2. Access the dashboard to manage students
3. Add, edit, or delete student records
4. Track progress with exam results
5. Filter and search students by various criteria

## Project Structure

```
student_progress/
├── dashboard/              # Django app for student management
│   ├── migrations/         # Database migration files
│   ├── templates/          # HTML templates
│   ├── admin.py           # Django admin configuration
│   ├── apps.py            # App configuration
│   ├── models.py          # Database models
│   ├── tests.py           # Test cases
│   └── views.py           # View functions
├── student_progress/       # Main project settings
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py        # Project settings
│   ├── urls.py            # URL configurations
│   └── wsgi.py
├── manage.py              # Django management script
├── README.md              # This file
└── .gitignore             # Git ignore configuration
```

## Key Functionality

- **Student Management**: Add, edit, delete, and view student records
- **Progress Sheets**: Track quarterly, midterm, model, and end-term exam results
- **Multi-Subject Tracking**: Mathematics, Science, and English scores
- **Filtering Options**: Filter students by exam type and class
- **Search Functionality**: Search students by name or roll number
- **Dashboard Analytics**: Overview of student statistics

## Security Features

- User authentication and authorization
- OTP verification for account creation
- Session-based login management
- Input validation and sanitization

## Customization

To modify the application:

1. Update `dashboard/models.py` to change data models
2. Modify `dashboard/views.py` to change business logic
3. Edit templates in `dashboard/templates/` to change UI
4. Update `dashboard/urls.py` to modify URL routing
