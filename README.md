Face Recognition Based Attendance Monitoring System
A Python-based smart attendance system that uses facial recognition to automate the process of marking attendance with an easy-to-use graphical interface (GUI).

Overview
This system captures a user’s face through a webcam, identifies the person using a trained deep learning model, and marks attendance in real-time. It provides a secure, scalable, and user-friendly solution for managing attendance records for both students and admins.

Admins have extra privileges such as adding/removing users, managing attendance data, and modifying user credentials.

Features
Face recognition using a trained model.h5

Admin & student role support

Attendance marking only during scheduled times

Daily attendance reports in CSV format

Login authentication with default admin credentials

Secure registration of new users with role selection (student/admin)

Real-time date & time tracking

Live attendance table with updates on the GUI

Email notifications to absentees (optional extension supported)

Technologies Used
Technology	Purpose
Python	Core programming language
Tkinter	GUI development
OpenCV	Face detection & camera operations
Keras/TensorFlow	Deep learning model for face recognition
NumPy / Pandas	Data manipulation
CSV / Datetime	Attendance logging

Project Structure
Face Recognition Based Attendance Monitoring System/
│
├── main.py                       # Main application launcher
├── registration.py              # Register new users
├── model.h5                     # Trained face recognition model
├── img.png                      # Image used in GUI
│
├── Attendance/                  # Folder with daily attendance CSVs
│   ├── Attendance_25-04-2025.csv
│   ├── ...
│
├── StudentDetails/              # Stores registered user details
│   └── StudentDetails.csv
│
├── README.md                    # Project documentation
└── __pycache__/                 # Python cache files

How to Run the Project
Install dependencies:
pip install opencv-python numpy pandas tensorflow

Run the main application:
python main.py

Register new user (student/admin) via the GUI.

Mark attendance by detecting a registered face during scheduled lecture times.

Future Improvements
Integration with databases (SQLite/MySQL)

Support for cloud-based attendance syncing

Mobile camera face recognition

Enhanced security (encryption, 2FA)

Notification system for absentee reporting

Acknowledgements
OpenCV for computer vision tools

TensorFlow/Keras for model training

Python community for open-source libraries

