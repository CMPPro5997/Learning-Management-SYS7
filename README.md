 Introduction 
This report is for my learning management system.
 Project Aim: To produce a learning management system that shows full functionality in terms of user roles student, admin, and teacher.
 The technologies I used were:
•	React
•	Django
•	Django REST Framework
•	SQLite
•	Python
 System Architecture 
1.	Frontend Layer
•	I developed this using React.
•	I provided interfaces for students, teachers and administrators.
•	I ensure that the front end layer will send requests to the Django REST API.
2.	Backend Layer
•	I developed the back end using Django and Django REST Framework.
•	The back end layer will handle: authentication, course management, enrolments, lessons and quizzes.
•	There are process requests from the frontend.
3.	 Database Layer
•	SQLite database.
•	Stores users, courses, lessons, quizzes and enrolments.
•	Accessed through Django's ORM.
 Database Design 
 User Roles 
•	Student
•	Teacher
•	Admin
 API Endpoints 
 Testing 
 Screenshots 
 <img width="608" height="331" alt="image" src="https://github.com/user-attachments/assets/31667dfa-d474-43a6-8079-01c5dfe6a9d9" />
Figure 1: Student Authentication Page
 <img width="563" height="669" alt="image" src="https://github.com/user-attachments/assets/7ff9f022-68d4-42c5-b125-f21ece3cba39" />

Figure 2 Student dashboard showing enrolled courses.

 

Teacher Screens
 <img width="940" height="531" alt="image" src="https://github.com/user-attachments/assets/9d453ed1-c873-49c1-9661-69458d6b4505" />

Figure 3: This is the screen the teacher1 sees when they login
 <img width="940" height="674" alt="image" src="https://github.com/user-attachments/assets/c7014e59-90cf-4254-b66d-223244fd0bb1" />

Figure 4: teacher1 courses

 <img width="940" height="775" alt="image" src="https://github.com/user-attachments/assets/18df1f92-2d25-48ca-94d3-41648dc8f23a" />

Figure 5: teacher 1 lessons
 <img width="940" height="648" alt="image" src="https://github.com/user-attachments/assets/56583437-9746-4deb-b1b4-ee4171d8a16a" />

Figure 6: quizzes
 Student screens
  <img width="323" height="290" alt="image" src="https://github.com/user-attachments/assets/e7da260d-7559-492a-affc-2c2287d6a01a" />
<img width="356" height="314" alt="image" src="https://github.com/user-attachments/assets/03812a41-ad44-423d-af24-41fc5c6a3dfb" />
<img width="425" height="338" alt="image" src="https://github.com/user-attachments/assets/f302dc68-2057-49e3-b3fe-689b35e2b579" />

 <img width="940" height="714" alt="image" src="https://github.com/user-attachments/assets/0db7083a-4cbf-4a2b-889c-44e67b2a9308" />
<img width="940" height="821" alt="image" src="https://github.com/user-attachments/assets/97e221c5-733a-410b-8d9d-fbf62c8960f7" />

Figure 7 administrator screen
 
Figure 8: Permissions set by admin for teachers and student privilege levels
The LMS uses SQLite as the relational database.
Main tables:
•	Users
•	Courses
•	Lessons
•	Quizzes
•	Enrolments
Relationships:
•	One Teacher can create many Courses
•	One Course can contain many Lessons
•	One Course can contain many Quizzes
•	One Student can enroll in many Courses

1.	Testing 
Feature Tested	Result
Student Login	Pass
Student Dashboard	Pass
Course Viewing	Pass
Teacher Login	Pass
Course Creation	Pass
Lesson Creation	Pass
Quiz Management Structure	Pass
Admin Login	Pass
User Management	Pass
Enrolment Management	Pass

+------------------+
| React Frontend |
+------------------+
|
v
+------------------+
| Django REST API |
+------------------+
|
v
+------------------+
| SQLite Database |
+------------------+

Conclusion
Quiz functionality has been partially implemented within the backend structure. Due to project timescales, full student quiz interaction and assessment tracking were identified as future enhancements. The current LMS successfully delivers user authentication, course management, lesson management, role-based access control and student enrolment functionality.

