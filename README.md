MedTrack: A Cloud-Enabled Healthcare Management System<br>
Project Description<br>
MedTrack is a cloud-based healthcare management system designed to streamline patient-doctor interactions. It enables patients to book appointments, manage medical histories, and receive diagnoses online. Built using Flask for backend development, AWS EC2 for hosting, and DynamoDB for data management, the system ensures secure and efficient healthcare management.

Features<br>
User Registration & Authentication (Doctors & Patients) <br>
Appointment Booking System<br>
Secure Data Storage with AWS DynamoDB<br>
Real-time Notifications<br>
IAM-Based Role Management for Secure Access<br>
Cloud Hosting on AWS EC2<br>
Flask Backend with Boto3 Integration<br>
Responsive Web Pages for Easy Navigation<br>

Tech Stack<br>
Backend: Flask (Python)<br>
Database: AWS DynamoDB<br>
Hosting: AWS EC2<br>
Security: AWS IAM (Identity & Access Management)<br>
Version Control: Git/GitHub<br>
Frontend: HTML, CSS<br>

Setup & Installation<br>
Prerequisites<br>
AWS Account (For EC2, DynamoDB, IAM)<br>
Python3 & pip<br>
Flask Framework<br>
Boto3 for AWS Integration<br>
Git for Version Control<br>

Installation Steps<br>
1. Clone the Repository<br>
git clone <repository-url>
cd MedTrack
2. Set up a Virtual Environment<br>
python3 -m venv venv
source venv/bin/activate
3. Install Dependencies<br>
pip install -r requirements.txt
4. Configure AWS Credentials<br>
Set up AWS IAM roles for secure access.
Update config.py with AWS access credentials.
5. Run the Application Locally<br>
python app.py
Access the application at http://127.0.0.1:5000/


Deployment on AWS EC2<br>
1. Launch EC2 Instance<br>
Choose Amazon Linux 2 or Ubuntu as the AMI.<br>
Open ports for HTTP (80) & SSH (22).<br>
2. Connect to EC2 Instance<br>
ssh -i <your-key.pem> ec2-user@<your-instance-public-ip><br>
3. Set Up the Environment<br>
sudo yum update -y<br>
sudo yum install python3 -y<br>
sudo pip3 install virtualenv<br>
python3 -m venv venv<br>
source venv/bin/activate<br>
pip install flask boto3<br>
4. Deploy the Flask Application<br>
python app.py<br>
5. Access the Web App<br>
http://<EC2-Public-IP>:5000<br>

Project Workflow
1. AWS Account Setup & IAM Configuration
2. DynamoDB Table Creation
3. Flask Backend Development
4. EC2 Instance Deployment
5. Testing & Debugging
6. Production Deployment

User Guide<br>
For Patients:<br>
Register/Login<br>
Book Appointments<br>
View Medical History<br>
Receive Diagnosis Reports<br>

For Doctors:<br>
Login to the Dashboard<br>
View Patient Appointments<br>
Submit Diagnoses & Treatment Plans<br>

Database Schema<br>
Users Table<br>
Appointments Table<br>

Testing<br>
Functional Testing: User registration, login, appointment booking<br>
Database Testing: Data retrieval from DynamoDB<br>
Security Testing: AWS IAM Role-Based Access<br>

Conclusion<br>
MedTrack is a scalable, secure, and efficient cloud-based healthcare management system. By leveraging AWS services, it enhances patient-doctor interactions, streamlining the process of appointment booking and medical data management.
