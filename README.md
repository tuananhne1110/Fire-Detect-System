# Fire Detection System

## Overview
The Fire Detection System is a comprehensive solution designed to detect fire through various sources, including images, videos, and real-time camera feeds. This system leverages advanced machine learning models to identify fire with high accuracy and provides a user-friendly interface for monitoring and detection.

## Features
1. Image and Video Detection
     - Upload images or videos to detect the presence of fire.
     - Visual indication of detected fire regions in the uploaded media.

2. Live Camera Detection
     - Real-time fire detection using live camera feeds.
     - Switch between IP cameras and Webcam for flexible monitoring.
     - Continuous monitoring with instant alerts on fire detection.
     - Email Notifications: When fire is detected in the live feed, an email notification with evidence (snapshot of the detected fire) is sent to the user's email.
  
## Installation
To install and run the Fire Detection System, follow these steps:

**Prerequisites
Python 3.8 or higher
Virtual environment tools (optional but recommended)
Required Python packages listed in 'requirements.txt'

**Steps
1. Clone the Repository
"""
   git clone https://github.com/yourusername/fire-detection-system.git
   cd fire-detection-system"""
   
2. Create and Activate Virtual Environment (Optional)
  python -m venv venv
  source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install Dependencies
   pip install -r requirements.txt

4. Run the Application
   python app.py

## Usage
1. Image and Video Detection
    - Open the web application in your browser.
    - Navigate to the Image/Video Detection section.
    - Upload an image or video file.
    - The system will process the file and display the result with highlighted fire regions if detected.

2. Live Camera Detection
    - Open the web application in your browser.
    - Navigate to the Live Camera Detection section.
    - Select the camera source (IP Camera or Webcam).
    - If using an IP Camera, enter the IP address and connect.
    - The system will start the live feed and begin detecting fire in real-time.
    - Switch between IP Camera and Webcam as needed.
    - If fire is detected in the live feed, an email notification with a snapshot of the fire will be sent to the configured email address.

## Email Notification Setup
To set up email notifications, update the config.py file with your email credentials and recipient address:

# Email Configuration
email_flag = 0
smtp_port = 587
smtp_server = "smtp.example.com"
email_from = "your_email@example.com"
email_list = ["recipient@example.com"]
pswd = 'your_password'
subject = "mail_subject"
formatted_time = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
