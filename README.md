# Facial Recognition Attendance System (Flask)

A modern, web-based facial recognition attendance system designed for educational institutions. This application leverages deep learning to automate attendance marking through real-time video streams, providing a seamless experience for both students and faculty.

## ✨ Features
*   **Real-Time Recognition**: Mark attendance instantly using live video.
*   **Role-Based Dashboards**: 
    *   **Students**: View individual attendance history and download records.
    *   **Faculty**: Manage student registrations, view overall attendance, and track metrics.
*   **Admin Settings**: Dedicated administrator panel to clear system data (students/attendance) while preserving staff information.
*   **Glassmorphism UI**: A premium, modern dark-mode interface with frosted glass effects and smooth animations.
*   **Data Export**: Download attendance reports in CSV format.

## 🛠️ Technology Stack
*   **Backend**: Python (Flask), Flask-SQLAlchemy (SQLite)
*   **Computer Vision**: OpenCV, Face-Recognition (dlib)
*   **Frontend**: Bootstrap 4, FontAwesome, Custom Glassmorphism CSS
*   **Database**: SQLite

## 🚀 Getting Started

### Prerequisites
*   Python 3.12+ (Recommended)
*   Webcam (for registration and attendance)

### Installation
1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/Srinidhi14062005/Specialization-Hackathon.git
    cd facial-recognition-attendance-webapp
    ```

2.  **Install Dependencies**:
    *Notes: On Windows, you may need Visual Studio C++ build tools for `dlib`.*
    ```bash
    pip install flask flask-sqlalchemy opencv-python numpy face_recognition dlib
    ```

### Initializing the Database
The project automatically initializes the database upon the first run. To add an administrator account, you can run the included setup script:
```bash
python add_admin.py
```
*Current Default Admin: `admin@dev.com` / `admin123`*

### Running the Project
Start the Flask development server:
```bash
python -m flask run --debug
```
Access the application at: **http://127.0.0.1:5000**

## 📂 Project Structure
*   `app.py`: Main application logic and routing.
*   `models.py`: Database models (Student, Faculty, Attendance).
*   `video_capture.py`: Background video processing utility.
*   `static/`: CSS, images (profile pictures), and JS files.
*   `templates/`: HTML structures using Jinja2 templates.
*   `db/`: SQLite database storage.

---
© 2026 FR-Attendance System
