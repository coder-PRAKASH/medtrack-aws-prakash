

# MedTrack 🏥 (AWS Cloud-Based Healthcare System)

MedTrack is a cloud-enabled healthcare management system built using Flask and AWS services.
It allows patients to book appointments with doctors, manage medications, and receive automated notifications.

The application integrates AWS DynamoDB for data storage and AWS SNS for email notifications.

📂 Project Structure
medtrack/
│
├── app.py                    # Main Flask application
├── requirements.txt          # Python dependencies
│
├── templates/                # HTML templates
│   ├── aboutus.html
│   ├── addmedication.html
│   ├── appointment.html
│   ├── contactus.html
│   ├── doctordashboard.html
│   ├── doctorreview.html
│   ├── index.html
│   ├── login.html
│   ├── patientdashboard.html
│   ├── patientreview.html
│   ├── prescribe.html
│   └── signup.html
│
├── static/
│   └── styles.css            # CSS styling

🛠️ Setup Instructions

Follow these steps to run the project locally.

1️⃣ Clone the Repository
git clone https://github.com/coder-PRAKASH/medtrack-aws-prakash.git
cd medtrack-aws-prakash

2️⃣ Create Virtual Environment

Linux / Mac

python3 -m venv venv

Windows

python -m venv venv


3️⃣ Activate Virtual Environment

Linux / Mac

source venv/bin/activate

Windows

venv\Scripts\activate

4️⃣ Install Dependencies
pip install -r requirements.txt
5️⃣ Run the Application
python app.py

Server will start at:

http://127.0.0.1:5000

☁️ AWS Setup

To enable cloud features, configure AWS services.

DynamoDB Tables

Create the following tables:

Users Table

Primary Key: email (String)

Appointments Table

Primary Key: id (String)

Medications Table

Primary Key: id (String)

Prescriptions Table

Primary Key: id (String)
SNS Topic

Create an SNS topic:

MedTrackNotification

Subscribe your email to receive appointment notifications.

🚢 Deployment (Optional)

For production deployment on AWS EC2:

pip install gunicorn
gunicorn --bind 0.0.0.0:8000 app:app
💻 Technologies Used
Backend

Python

Flask

Cloud Services

AWS DynamoDB

AWS SNS

Frontend

HTML

CSS

📧 Notification System

When a patient books an appointment:

Appointment is stored in DynamoDB

SNS publishes a notification

Email is sent to subscribed users
## 👤 Author
Prakash  
GitHub: https://github.com/coder-PRAKASH
## 🚀 My Contributions

- Worked on project setup and execution  
- Learned and implemented AWS services (DynamoDB, SNS)  
- Uploaded and managed project on GitHub  


