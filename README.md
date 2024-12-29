#**Smart Attendance System**

This project is a Smart Attendance System that utilizes Python and OpenCV to automate the process of attendance marking. The system captures images of individuals using a camera, extracts features, and compares them with pre-stored images in the database to verify identities and mark attendance.

**Features**

Collect Face Datasets: Capture face images using a camera for training.

Extract Facial Features: Convert face images into feature vectors for comparison.

Automated Attendance Marking: Recognize faces in real-time and mark attendance automatically.

Web-Based Database Management: Use a Flask-based web interface to view and manage attendance records.

**Technologies Used**

OpenCV: For real-time face detection and recognition.

dlib: For facial feature extraction.

Flask: To create a web-based interface for managing attendance records.

Pandas: For managing attendance data in tabular format.

NumPy: For numerical operations.

scikit-image: For image preprocessing.

**Setup and Installation**

Prerequisites:

Ensure you have Python 3.7 or higher installed on your system.

Install the required Python packages using the following command:

pip install -r requirements.txt

**Required Libraries**

dlib==19.17.0

numpy==1.22.0

scikit-image==0.18.3

pandas==1.3.4

opencv-python==4.5.4.58

flask

**Usage**

Step 1: Collect Face Dataset

Run the following script to collect face images for the dataset:

python get_faces_from_camera_tkinter.py

This script captures face images from the camera and saves them in a designated folder for training.

Step 2: Extract Features

Convert the collected dataset into feature vectors by running:

python features_extraction_to_csv.py

This script processes the face dataset and stores the extracted features in a CSV file.

Step 3: Take Attendance

Use the following script to mark attendance based on face recognition:

python attendance_taker.py

The script recognizes faces in real-time and marks attendance in the database.

Step 4: Check the Database

Launch the Flask application to manage and view attendance records:

python app.py

Access the web interface at http://localhost:5000 to check and manage attendance records.


**Screenshots**

![Screenshot 2024-12-29 215338](https://github.com/user-attachments/assets/8591cc5d-58cc-4d5e-97bb-7d6b789b2ec1)

![Screenshot 2024-12-29 215033](https://github.com/user-attachments/assets/1e61f300-f9ff-4554-9912-fa7af88e0f11)








