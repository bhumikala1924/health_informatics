# health_informatics
## Description  The Maternal and Child Health Tracking System is a web-based healthcare application developed to improve the monitoring and management of maternal and child health services. The system digitizes patient records and helps healthcare workers track ANC, delivery, PNC, and immunization services.
# problem statement 
## Many healthcare facilities still use paper-based systems for maternal and child health records. These systems create several challenges, including:

- Loss or damage of patient records
- Difficulty in tracking pregnant women and children
- Missed vaccination schedules and appointments
- Delayed reporting and decision-making
- Lack of proper communication between health workers and patients
- Inaccurate data management and duplication
  therefore, a computerized maternal and child health trackimg system is needed to improve record management, monitoring, and healthcare delivery.

 # OBJECTIVES
 # GENERAL OBJECTIVE 
 To develop a digital Maternal and Child Health Tracking System for improving healthcare service delivery, monitoring, and follow-up of pregnant women and children.
 # SPECIFIC OBJECTIVES 
 Register and maintain records of pregnant women.
Track Ante-Natal Care (ANC) services.
Manage delivery and Post-Natal Care (PNC) services.
Register children and monitor immunization schedules.
Generate reminders and notifications through SMS.

# LITERATURE REVIEW 
Maternal and child health is an important public health issue, particularly in developing countries. Studies have shown that digital health information systems improve healthcare services by maintaining accurate records, tracking ANC and immunization schedules, and sending reminders to patients. Mobile technologies such as SMS notifications further enhance communication between healthcare workers and patients.

# SYSTEM FEATURES 
Pregnant Women Registration
Child Registration
ANC Tracking
Delivery Management
Postnatal Care Tracking
Immunization and Vaccination Tracking
Appointment Scheduling
SMS Reminder Notifications

# METHODOLOGY 
1.Requirement Analysis

Identify the requirements of healthcare workers and users.

2. System Design

Design the user interface, database, and workflow of the system.

3. System Development

Develop the application using suitable technologies.

4. Testing

Test the system for functionality, reliability, and security.

5. Implementation

Deploy the system and provide training to healthcare staff.

6. Maintenance and Evaluation

Monitor performance and update the system when necessary.

# SYSTEM DESIGN 
*Actors
Administrator
Healthcare Worker
Patient
*Main Processes
Mother Registration
Child Registration
ANC Monitoring
Delivery Tracking
PNC Monitoring
Vaccination Tracking
SMS Notifications

# TOOLS AND TECHNOLOGIES
| Component            | Technology              |
| -------------------- | ----------------------- |
| Frontend             | HTML, CSS, Bootstrap    |
| Backend              | Django                  |
| Programming Language | Python                  |
| Database             | MySQL                   |
| Platform             | Web-based System        |
| Additional Tool      | SMS Notification System |

# ER DIAGRAM
                           +----------------------+
                           |       MOTHER         |
                           +----------------------+
                           | PK Mother_ID         |
                           | Name                 |
                           | Age                  |
                           | Address              |
                           | Phone_Number         |
                           | Blood_Group          |
                           | Registration_Date    |
                           +----------------------+
                                   |
              -------------------------------------------------
              |                    |                  |       |
             1:M                  1:M                1:M     1:M
              |                    |                  |       |
     +---------------+    +---------------+   +--------------+  +----------------+
     |      ANC      |    |    DELIVERY   |   |     PNC      |  |     CHILD      |
     +---------------+    +---------------+   +--------------+  +----------------+
     | PK ANC_ID     |    | PK Delivery_ID|   | PK PNC_ID    |  | PK Child_ID    |
     | FK Mother_ID  |    | FK Mother_ID  |   | FK Mother_ID |  | FK Mother_ID   |
     | Visit_Date    |    | Delivery_Date |   | Visit_Date   |  | Name           |
     | Weight        |    | Delivery_Type |   | Health_Status|  | Gender         |
     | BloodPressure |    +---------------+   +--------------+  | Date_of_Birth  |
     +---------------+                                          +----------------+
                                                                        |
                                                                       1:M
                                                                        |
                                                         +--------------------------+
                                                         |       VACCINATION         |
                                                         +--------------------------+
                                                         | PK Vaccine_ID            |
                                                         | FK Child_ID              |
                                                         | Vaccine_Name             |
                                                         | Date_Given               |
                                                         | Next_Dose_Date           |
                                                         +--------------------------+
                                                         
                                                         
                                                         
  # INSTALLATION GUIDE
  ## Installation Guide

1. Clone the repository from GitHub.
2. Navigate to the project directory.
3. Install the required dependencies.
4. Configure the database.
5. Run the Django server.
6. Access the application through a web browser.

# FUTURE SCOPE 
Mobile Application Support
Cloud-Based Storage
Dashboard and Data Analytics
Email Notifications
Integration with HMIS
AI-Based Risk Prediction

# CONTRIBUTORS
bhumikala chaudhary 
samiksha thapa
sushreeka khadka 
susmita mahat

