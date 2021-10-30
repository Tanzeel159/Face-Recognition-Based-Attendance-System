## Face-Recognition-Based-Attendance-System

![facial-recognition-icons-collection_1268-7075](https://user-images.githubusercontent.com/20295349/120059277-11a69f00-c06e-11eb-8ce1-59d16c28d026.jpg)


### Table of Contents
-  [Introduction](#introduction)
-  [System Analysis](#system-analysis)
-  [Proposed System](#proposed-system)
-  [Requirements](#requirements)
-  [Algorithm](#algorithm)
-  [Implementation](#implementation)
## Introduction 
Attendance is primarily important for both the teacher and student of an educational organization.It is very important to keep record of the attendance. The problem arises when we think about the traditional process of taking attendance in class room which involves calling name/roll number. This process is time consuming.A face recognition based attendance system could automate the entire system and streamline the process increasing the rate and reducing the time.

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

- To add student details and capture images for dataset
```
python add_student.py
```
![addstudent](https://user-images.githubusercontent.com/20295349/120060773-4408ca00-c077-11eb-9f77-2bbe5ff456ef.PNG)

- Dataset folder consisting of images(Anand)

 ![image](https://user-images.githubusercontent.com/20295349/120061621-b54a7c00-c07b-11eb-94eb-cc886affb1ad.png)

- Folder of images in dataset

![image](https://user-images.githubusercontent.com/20295349/120061633-c1ced480-c07b-11eb-9734-634823dbd983.png)
```
python create_person.py
```
![personid](https://user-images.githubusercontent.com/20295349/120061768-53d6dd00-c07c-11eb-903d-a400f9ae6c09.PNG)

```
python add_person_faces.py
```
![URL](https://user-images.githubusercontent.com/20295349/120061823-96001e80-c07c-11eb-91bd-fb6fd73ea398.PNG)
```
python train.py
```
![train](https://user-images.githubusercontent.com/20295349/120061863-c8118080-c07c-11eb-90d1-437857e5df5e.PNG)
```
python get_status.py
```
![status](https://user-images.githubusercontent.com/20295349/120061881-e1b2c800-c07c-11eb-9af1-7a8fe799c999.PNG)
```
python detect.py ./pics/test.jpg
```
![detect](https://user-images.githubusercontent.com/20295349/120061914-0eff7600-c07d-11eb-9180-6b6e578a3668.PNG)
![image](https://user-images.githubusercontent.com/20295349/120061934-25a5cd00-c07d-11eb-9db7-9be0501ffca3.png)
- Image used for detecting faces
```
python spreadsheet.py
```
![spreadsheet](https://user-images.githubusercontent.com/20295349/120061969-48d07c80-c07d-11eb-8623-2bd9367139b3.PNG)
```
python identify.py
```
![4](https://user-images.githubusercontent.com/20295349/120062011-7c130b80-c07d-11eb-8322-c6bf1d1c70b7.PNG)
![3](https://user-images.githubusercontent.com/20295349/120062019-8503dd00-c07d-11eb-9a4d-54076c5232d3.PNG)
![5](https://user-images.githubusercontent.com/20295349/120062676-0446e000-c081-11eb-886d-2710aa6acefb.PNG)


[Back to the Top](#table-of-contents)
