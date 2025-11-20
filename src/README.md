# Mergington High School Activities

A FastAPI web application that allows teachers to manage student participation in extracurricular activities at Mergington High School.

## Features

### Student Activity Management
- View all available extracurricular activities with detailed information
- Sign up students for activities (requires teacher authentication)
- Unregister students from activities (requires teacher authentication)

### Advanced Filtering and Search
- Search activities by name
- Filter by category (Sports, Arts, Academic, Community, Technology)
- Filter by day of the week
- Filter by time range (Before School, After School, Weekend)

### Teacher Authentication
- Secure teacher login system
- Session management for authenticated users
- Role-based access (teacher and admin roles)

### Activity Information
- Activity descriptions and schedules
- Participant tracking
- Maximum capacity management
- Schedule details with days and times

## Technology Stack

### Backend
- **FastAPI**: Modern Python web framework for building APIs
- **MongoDB**: NoSQL database for storing activities and teacher information
- **Uvicorn**: ASGI server for running the application
- **Argon2**: Password hashing for secure authentication

### Frontend
- **Vanilla JavaScript**: Dynamic client-side functionality
- **HTML5/CSS3**: Modern, responsive user interface
- **Modal dialogs**: For login and registration flows

## API Endpoints

### Activities
- `GET /activities/`: Get all activities with optional filtering by day and time
- `GET /activities/days`: Get list of all days with scheduled activities
- `POST /activities/{activity_name}/signup`: Register a student for an activity
- `POST /activities/{activity_name}/unregister`: Remove a student from an activity

### Authentication
- `POST /auth/login`: Authenticate a teacher account
- `GET /auth/check-session`: Validate an active session

## Development Guide

For detailed setup and development instructions, please refer to our [Development Guide](../docs/how-to-develop.md).
