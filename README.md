## Face-Recognition-Based-Attendance-System

![facial-recognition-icons-collection_1268-7075](https://user-images.githubusercontent.com/20295349/120059277-11a69f00-c06e-11eb-8ce1-59d16c28d026.jpg)


### Table of Contents
-  [Introduction](#introduction)
-  [System Analysis](#system-analysis)
-







## Introduction 
Attendance is prime important for both the teacher and student of an educational organization.It is very important to keep record of the attendance. The problem arises when we think about the traditional process of taking attendance in class room which involves calling name/roll number. This process is time consuming.A face recognition based attendance system could automate the entire system and streamline the process increasing the rate and reducing the time.

[Back to the Top](#table-of-contents)
## System Analysis
Existing Systems include: 
- Scanning ID cards 

![image](https://user-images.githubusercontent.com/20295349/120060130-9647ec00-c073-11eb-9a1b-f0ec61e01e55.png)
- Using biometric systems 

![image](https://user-images.githubusercontent.com/20295349/120060141-a8c22580-c073-11eb-9ede-b911e5b23de1.png)
- Traditional Method 
In this approach teacher calls out the roll numbers of student to which students respond accordingly

[Back to the Top](#table-of-contents)
## Proposed System
Face Recognition Based System
- 20 images are captured for every user to create dataset.
- All the details related to student are captured in database.
- This information is converted to URL which is sent to Azure Cloud.
- Each person has unique Face ID.
- Faculty takes image and feeds to system after which the program analyzes the faces and marks attendance.

[Back to the Top](#table-of-contents)
## Requirements
![WINWORD_bTrJsW4C60](https://user-images.githubusercontent.com/20295349/120060530-f93a8280-c075-11eb-9473-e05959b9d802.jpg)


[Back to the Top](#table-of-contents)
## Algorithm
Azure Face API is used to detect, recognize and analyze human faces in images.
- Get Face Attributes
- Authorize the Face API Call
- Create the Person Group
- Define people for Person Group
- Detect faces and register them to correct person
- Train the Person Group
- Identify face against defined group

[Back to the Top](#table-of-contents)
## Implementation
- Setup virtual environment for the project
- Install all the dependency libraries such as OpenCV, Openpyxl, face_recognition,Dlib, cognitive_services, Sqlite3
![lib](https://user-images.githubusercontent.com/20295349/120060735-11f76800-c077-11eb-93cf-1575a17af63a.PNG)

- Execute add_student.py to add student details and capture images for dataset
![addstudent](https://user-images.githubusercontent.com/20295349/120060773-4408ca00-c077-11eb-9f77-2bbe5ff456ef.PNG)




