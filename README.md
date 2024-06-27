

# Online Project Manager
## Author: Ammar Elsherif

## Content:
1. INTRODUCTION  
1.1 Purpose  
1.2 Scope 
1.3 Definitions, Acronyms, and Abbreviations  
2. GENERAL DESCRIPTION  
2.1 Product Perspective  
2.2 Product Functions
2.3 User Characteristics
2.4 Operating Environment
2.5 Assumptions and Dependencies
3. SPECIFIC REQUIREMENTS 
3.1 External Interface 	Requirements
3.1.1 User Interfaces
3.1.2 Hardware Interfaces
3.1.3 Software Interfaces 
3.1.4 Communications Interfaces
3.2 Functional Requirements 
3.3 Use Cases 
3.4 Classes/Objects
3.5 Non-Functional Requirements
3.5.1 Performance
3.5.2 Reliability
3.5.4 Security
3.5.6 Portability
4. ANALYSIS MODELS 
4.1ERD
4.2 Use case
4.3 Sequence Diagrams4.4 Activity Diagram 
4.5 Deployment Diagrams 










#ACKNOWLEDGEMENT
I would like to thank Dr/ Walid for his guidance and patience. That made us
able to successfully construct this project “COOP System” to a matured
solution for posting questions safely online and seeking answers out of the daily
life experiences of the users. We are also thankful to Eng/ Doaa for her patience,
understanding, and guidance throughout the project.












# 1. Introduction 

## 1.1 Purpose 
<COOP> is an online project manager tool, <COOP> aims at providing individuals 
and teams with an efficient and user-friendly platform to organize and manage 
their tasks. The purpose of this system is to streamline task management 
processes, enhance collaboration among team members and improve overall 
productivity. By adopting the Kanban approach, the system allows users to 
visualize their workflow, limit work in progress, manage flow, make process 
policies explicitly, implement feedback loops and improve collaboratively. 
The Kanban approach is used in the system as a first release which guarantees flexible 
improving in the next releases like collaboration with another Agile approach according 
to the feedback from the market. 
The Kanban method has gained significant attention worldwide and is being used 
in various industries, ranging from small companies to large organizations. 
Here are some industries where the Kanban method can be used: 
-Manufacturing: The Kanban method originated in Japan and has been 
extensively used worldwide in diverse industries and manufacturing facilities. - 
Software Development: The Kanban approach is widely adopted in the software 
sector. 
-IT Operations: Kanban is also used in IT operations. 
-Engineering: The Kanban method finds application in engineering. Marketing: 
Many businesses use the Kanban method for marketing purposes. 
Regarding market studies about the demand for Kanban tools, a report suggests 
that the global Kanban tools market size was USD 234.7 million in 2021 and is 
expected to reach USD 761.2 million by 2028, exhibiting a CAGR of 18.0% during 
the forecast period. The COVID-19 pandemic has increased the demand for digital 
collaboration tools, including Kanban software, as remote work became more 
prevalent. The crisis highlighted the need for flexibility and adaptability, leading to 
enhanced features like virtual collaboration, task assignments, and progress 
tracking 

## 1.2 Scope 
Includes the development of an online platform that enables users to register and 
log in, create projects, and manage various components of the project. 
Administrators can create and modify project components, 
including story and task cards, assigning tasks to team members, tracking progress, and 
receive feedback and reports. Workers, on the other hand, can join existing 
projects, view project boards, access task cards assigned to them, mark tasks as 
completed, and communicate with team members through a chat space. 
The system's key functions include user authentication, project creation, task card 
creation, setting work-in-progress limits, messaging capabilities, task queue 
viewing, alerts for due dates, and performance measurement through cumulative 
charts. These functions aim to provide a comprehensive and integrated solution 
for effective task management and collaboration. 
By implementing this Online Task Management System, individuals and teams will 
benefit from improved organization, transparency, and accountability in their 
projects. It will enable effective communication, task tracking, and timely 
completion of deliverables. Additionally, the system will enhance productivity by 
providing insights into performance metrics and facilitating continuous 
improvement. 

## 1.3 Definitions, Acronyms, and Abbreviations 
There are a variety of terms used in this SRS relating to the software being created. 
Most of the terms are self-explanatory. However, for completeness, all terms 
related to the software are provided. 
 
 ### User: 
     An authenticated user on the system network who can 
    apply for an invitation to existing project/s on the system and/or 
    create his project, select the project team members from 
    the pool of other authenticated users, and fully utilize the 
    features applied for administration provided by <COOP> 

### Work in Progress (WIP):
   A term used in task management 
  systems to refer to time limitations for number of tasks or work 
  items that are currently in progress or being actively worked on 
  by individuals or teams. 
  
### Project:
   A visualized billboard contains a collection of cards 
  representing stories and tasks traveling through the phase 
  <Required>,<In progress>,<Done> all displayed on a dashboard 
  where teamwork selected from authenticated users 
  collaborate to get the whole work done. 
 
 ### Administrator: 
   A user who interacts with a project he/she 
  created on the system network, the Administrator controls the 
  whole project workflow members and the ability to terminate the 
  project.
  
 ### Worker:
   A user who applies for the project after receiving 
  an invitation and applying for it. 
  
 ### Reviewer: 
   A worker who has permission to drag the task 
  from the reviewing phase to the done phase. 
   Workflow board: It is the dashboard of the whole project, It 
  guarantees the whole teamwork can view the workflow of the 
  entire project. 
  
 ### Story Card: 
   The card created by the administrator represents a specific 
  requirement related to the project. 
 Task Card: It is a story card transformed into a task statement 
which specifies how requirements could be satisfied. 
 Requested: it is phase zero where the admin user creates 
his story cards, It is represented in a column. 

 ### In Progress: 
   It is the first phase of the task card and the second 
  in the entire process, It is represented in a column and splitter 
  into modes. 

 ### Task Mode:
   Modes of the task in the <In progress> phase are 
  <Working>,<Waiting>,<Reviewing>.
  
 ### Done:
   It is the final stage of the workflow where task cards got 
  verified by reviewers. 
 ### Database:
   The platform where all project tasks and users' data 
  are saved. 

  
# 2. General Description
   
## 2.1 Product Perspective 
The project's core idea is to develop an Online Task Management System that 
helps individuals and teams organize their tasks, set deadlines, and 
collaborate efficiently. The system will provide a user-friendly interface with 
features like: project whole frame creation, tracking, and monitoring which 
assumes providing basic features like task creation, assignment, progress 
tracking, notifications, and reporting. The <COOP> uses the Kanban approach 
and practices by pursuing incremental evolutionary changes and 
encouraging acts of leadership at all levels. <COOP> satisfies core Kanban 
practices by enabling users to: 

    -Create project 
    -Create requirements stories and transform them into tasks 
    -Visualize the workflow and control its components 
    -Limit work in progress -Manage flow 
    -Make process policies explicit 
    -Implement feedback loops 
    It should be developed to run on Windows, MacOS, and Linux devices. 
    
## 2.2 Product Functions 

• Register/Login – This is available for the unregistered users who wish to 
be allowed to contribute to the system’s community by either creating 
and managing a project or joining an existing one on the system network. 
•Create a project – This function is available for registered users, they can 
continue building and modifying the whole project components as the 
process continues. 
• Create story/task cards: The administrator user can build a story card that 
should be developed into a task card with extra details related to the task. 
In the requested/initial stage, the administrator must add a description, also 
can change the card color according to the related lane the story is part of. 
In the In Progress stage, the administrator user can nominate workers from 
the team to work on this task. It is open for both to access the task card 
core data like different attachment files, download and upload them also 
feedback and reporting issues are available for both users via a text input box 
in each card altered to a task worker can forward the card only within In 
progress column for reviewing stage only else the administrator can drag 
cards back or forward or deleting it. 
• Set WIP – This function is also only available for administrator users to set 
work in progress limit for <In Progress> column 
• Send/receive a message – This function is available for all team members 
in the project chat space to report a public issue or make an announcement. 
• View tasks queue – This function is available for workers to schedule tasks 
in progress that he/she is responsible for, prioritized by a sooner due date. 
• Get alerted – This function is available for workers to get alerted of the 
due date before the second and last quarter of the task's determined time. 
•Measure performance – This function is available for the whole 
team members, the user can view a cumulative chart of the 
process performance. 


## 2.3 User Characteristics 

### Project Managers: 
  These are individuals responsible for overseeing the planning, execution, and completion of projects. 
  They have a high-level view of the project and are responsible for 
  creating and managing project components, assigning tasks to 
  team members, and tracking overall progress.
  
### Team Members: 
  These are individuals who actively work on tasks 
  assigned to them within the project. They collaborate with other 
  team members, update task statuses, communicate progress, and 
  provide feedback on the tasks they are working on. 

### Administrators: 
  Administrators have elevated privileges within the 
  system. They have the authority to create and modify project 
  components, manage team members' access and permissions, 
  and make administrative decisions related to the project workflow. 
  Reviewers: Reviewers are team members who have the 
  responsibility of reviewing and verifying completed tasks before 
  they are marked as "done." They ensure that the tasks meet the 
  required standards and specifications. 
  
### Users with Different Technical Proficiency: 
  The system is designed to accommodate users with varying levels of technical proficiency, 
  from novice users to experienced individuals. The user interface 
  and interactions should be intuitive and user-friendly, allowing all 
  users to navigate and utilize the system effectively. 

### Collaborative Users: 
  The system caters to users who value collaboration and teamwork. They actively engage with other 
  team members, communicate through chat spaces, and provide 
  updates, and share relevant information to ensure a smooth project 
  execution.
  
### Time-Conscious Users: 
  Users of the system understand the 
  importance of time management and meeting deadlines. They 
  rely on the system to track task due dates, receive alerts, and 
  prioritize their work accordingly. 
### Goal-Oriented Users: 
  The system is used by individuals and teams who have specific goals and objectives to achieve. They leverage 
  the system's features to organize tasks, monitor progress, and work towards accomplishing their goals efficiently. 


## 2.4 Operating Environment 
  The Online Task Management System is designed to operate in the 
  following environment: 
  
  Operating Systems: Windows, MacOS, Linux 
  Web Browsers: Chrome, Firefox, Safari, Edge 
  Design Implementation Constraints 

## 2.5 The design and implementation constraints 
  Including: 
  ### Technology Stack: 
    The system is built using specific technologies 
    and frameworks, which may impose limitations on compatibility 
    with other technologies. 

### User Interface: 
  The user interface design should be responsive and 
  intuitive to ensure ease of use for users on different devices and 
  screen sizes. 
  
### Security: 
  The system should implement appropriate security 
  measures, such as encryption and user authentication, to protect 
  user data and prevent unauthorized access. 
  Performance: The system should be designed to handle 
  concurrent user activity and provide a responsive user experience, 
  even with a large number of users and tasks. 

## 2.6 Assumptions 
### Availability of Internet Connection: 
  Users are assumed to have a stable internet connection to access and use the system. 

### User Authentication: 
  Users are required to register and log in to 
  the system using valid credentials to access project features and 
  collaborate with team members. 
  User Roles: The system assumes the existence of user roles, such 
  as administrators, workers, and reviewers, with specific 
  permissions and responsibilities. 

### User Collaboration: 
  The system assumes that team members will 
  actively collaborate and communicate through the provided 
  messaging capabilities. 

### Data Storage: 
  The system assumes the availability of a reliable and 
  secure database to store project data, user information, and task 
  details. 

## 2.7 Dependencies 

The design and implementation of the Online Task Management, 
The system may have dependencies on the following factors: 
  -Third-Party Libraries and APIs:
  The system may utilize third-party libraries and APIs for specific functionalities, such as user 
  authentication, file uploading, and real-time messaging. 
  
  -Development Resources: 
  The successful implementation of the system may depend on the availability of development resources, 
  including skilled programmers, designers, and testers. 
  
  -System Integration:
  The system may need to integrate with other 
  existing systems or tools, such as email clients or project 
  management software, to enhance functionality and data 
  exchange. 
  
# 3. Specific Requirements
   
## 3.1 External Interface Requirements

### User Registration and Authentication: 

 -Users should be able to register for an account with a unique username and password. 
 -The system should authenticate users and provide secure access to their accounts. 

### User Roles and Permissions: 
 The system should support different user roles such as project 
 managers, team members, administrators, and reviewers. 
 Each user role should have specific permissions and access rights 
 within the system. 

### Project Creation and Management: 
 Users should be able to create new projects and define project 
details such as name, description, and due dates. 
 Project managers should have the ability to assign tasks, set 
priorities, and track overall project progress. 

### Task Management: 
 Users should be able to create tasks within a project, providing 
details such as task name, description, due date, and assigned 
team members. 
 Tasks should be sortable, filterable, and searchable based on 
various criteria such as status, priority, and assigned users. 
 Users should be able to update task status, add comments, and 
attach files to tasks. 

### Collaboration and Communication: 
 The system should provide real-time messaging or chat 
functionality for team members to communicate and collaborate 
on tasks. 
 Users should receive notifications and alerts for task assignments, 
updates, and approaching deadlines. 

### Document and File Management: 
 Users should be able to upload and attach files to tasks, such as 
documents, images, or other relevant files. 
 The system should support file versioning and provide options for 
downloading, previewing, and managing attached files. 

### Reporting and Analytics: 
 The system should generate reports and provide analytics on 
project progress, task completion rates, and user productivity. 
 Users should be able to view graphical representations of data, 
such as charts or graphs, to gain insights into project performance. 

### Mobile Accessibility: 
 The system should have a responsive design that is accessible and 
optimized for mobile devices, allowing users to manage tasks on 
the go. 

### Security and Privacy: 
 The system should implement appropriate security measures to 
protect user data, such as encryption of sensitive information and 
secure authentication protocols. 
 Users should have control over the privacy settings of their tasks 
and projects, determining who can access and view their 
information. 

### 3.1.1 Hardware Interfaces 
• There need not be any special hardware interfaces in the program, and 
the program may rely solely on the host operating system’s ability to load 
the website. 
• Minimal hardware capabilities are required, any device with a proper 
browser can load the system. 

### 3.1.3 Software Interfaces 
• <> requires a browser that supports JavaScript. 
• The software is connected to SQL databases. 
• All databases for the software will be configured. These databases include 
Users’ credentials, posted questions and commented answers. 

### 3.1.4 Communications Interfaces 
This system supports all types of web browsers and requires internet connection to be loaded 
and accessed 

### 3.1.2 User Interfaces 
Login Interface: 
Profile interface 
Project board interface:







Task Card Pop-up Interface:


Project cumulative chart interface:
 


## 3.2 Functional Requirements

### 3.2.1 <Create project> 

Administrator users can create a project, set a name, description, and 
purpose, select the project's team members from the pool of  
authenticated users of the system, and name reviewers. Creation results in 
a basic layout that contains a basic implementation of the Kanban 
manufacturing process including the 3 main columns on the Kanban board 
[requested, in progress, done]. It is a must to set WIP limitations in the 
creation process. 

### 3.2.2 <create story card> 
Admin users can create a card that represents a single story of a feature or a 
single requirement. it contains the requirement description, date of 
creation, author, date of last modification. The story card is ready then to 
inherit one or more task cards related to the requirement assigned in the 
story card. Also selecting a specific color for the is guaranteed to divide 
different requirements and their related tasks into lanes which helps in 
organizing parallel work processing and managing. 

### 3.2.3<build task> 
 It occurs when the admin user drags a single story card from 
one column into another, the < Story Card> inherits a . contains a Reporting text 
box for managers and workers to use in reporting and feedback and drive 
space to send/receive task files to/from the worker. For complete building 
of the task, it is required from the user the following: 

	-A description of the task. -Attachments related to the task. 
	-Assign a member/s that is responsible for the task. 
	-Select reviewers from nominated workers. 
	-optionally user can set time limitations of the task. 
Along the journey from the beginning in phase passes through 3 modes, and the admin has 
authority for full control of phases and modes by dragging it right or back to left, otherwise, can 
only drag the card from mode into mode while the reviewer can only drag the card from waiting to 
reviewing and just alerts the admin of reviewing being finished using the reporting text box in the 
note: setting a WIP limit for individual tasks can lead to suboptimal results if not managed 
properly. It can lead to delays in completing tasks and may not be effective in identifying 
bottlenecks 

### 3.2.4 Delete card
 This functionality is only available for the admin of the project 
either by deleting a single or by deleting multiple related tasks by deleting the source . 

### 3.2.5 Create Alarm
This functionality is for all users but is specified according to their 
different roles for example: when a user administrates some project he/she gets alarmed before the 
half and the last quarter of duration is passed. The same occurs for the user whose role is a 
worker (or reviewer) he/she gets alarms of tasks queued that he/she is responsible for. 

### 3.2.6 Get a notification
 All kinds of users should be notified of every action/update 
occurs in the project all according to their roles.

### 3.2.7 Send message
 All kinds of users should be able to send/receive messages in the 
chat space of the project. 

### 3.2.8 Get task queue
 If the user is included in a project as a worker (or indifferent 
projects) then he/she gets a scheduled queue of tasks prioritized by the closer due date. 

### 3.2.9 View performance
All kinds of users involved in the project should be able to 
view a cumulative chart of the progress performance. 


## 3.3 Use Cases 
  1- User can register an account, all accounts have accessibility to create or/and join one or more projects.
  2- The user can monitor all projects that he/she joined/created.
  3- If  the user is an admin then he/she can create stories, develop them into tasks, modify, and delete them.
  4-If the user is an admin then he can assign other project member users as reviewers who (also the admin) can 
  move tasks from the reviewing phase to either the done phase or another previous phase.
  
## 3.4 Classes/Objects 

### 3.4.1 <user> 
#### 3.4.1.1 Attributes 
  • Name 
  • ID 
  • Password 
  • Projects_owned 
  • projects_joined 
  • Activity_log 
  • E_mail 
  • Phone 
  • Job 
  • tasks 
  
#### 3.4.1.2 Functions 
 Sign_up() 
 Login() 
 Create_project() 
 Search_member() 
 Access_project() 
 Select_member() 
 Create_card() 
  Build_task(card.cid) 
  Drag_card(card.cid) 
  Delete_card() 
 Update_card(card.cid) 
 Report(card.cid) 
 Terminate_project() 
 Send_msg() 
 Get_queue(self.id) 
 Get_alarm()
 
### 3.4.2 <project> 
#### 3.4.2.1 Attributes: 
 Pid Title 
 Description 
 Admin_name 
 Admin_id 
 Team_members_id, 
 WIP 
 WIP_ratio 
 
#### 3.4.2.2 Functions 
 Get_project_info() 
 get_permission() 
 notify_user(user.id) 
### 3.4.3 <Story card> 
#### 3.4.3.1 Attributes 
 Cid 
 Title 
 Story 
 date_added 
 date_last_modified 
 Color 
 author_id 

#### 3.4.3.2 Functions 
 Get_card_info() 
 Set_card_info( 
### 3.4.4 <task card> 
#### 3.4.4.1 Attributes 
 Tid 
 Title 
 Required 
 Data 
 Reports 
 date_added 
 date_last_modified 
 date_deadline 
 Phase 
 Mode 
#### 3.4.4.2 Functions 
 Get_card_info() 
 Set_card_info() 
 Get_card_data() 
 Set_card_data() 
 Set_phase() 


## 3.5 Non-Functional Requirements 
### 3.5.1 Performance 
• Any operation that is expected to take 0.1s or less shall not post any wait indicator. 
• Any operation that is expected to take more than 0.1s, but less than 1s, shall post the system wait 
cursor. 
• Any operation that is expected to take 1s or more shall post a progress bar, count-down timer, or 
another system-appropriate wait/progress indicator. 
• System downtime may not exceed 1 minute per day. 
• 95% of transactions shall be processed in less than a second. 

### 3.5.2 Reliability 
All posts and comments can be accessed anytime anywhere. 
3.5.3 Security. 
• All users’ passwords must be at least 8 characters and they must contain Upper case letters, lower case 
letters, and numbers, but also it can contain special characters. 

• All users’ credentials that are stored in the database are encrypted and no one can access it if 
anybody can access it then they won’t be able to read or use it as it is encrypted. 

### 3.5.4 Portability 
The system can be accessed anytime and anywhere as long as there’s a modern browser that supports JavaScript the proper internet connection and the minimal hardware requirements.

## 3.6 Logical Database Requirements 
• The system can store the following data: X 
• The system will maintain a backup database.  


# 4. ANALYSIS MODELS 

## 4.1 ERD


## 4.2 Use cases


## 4.3 Sequence Diagrams

## 4.4 Activity Diagram
![Activity diagra](/ActivityDiagram.drawio.png "Activity Diagram")

![Activity diagra](/ActivityDiagram.drawio1.png "Activity Diagram")

![Activity diagra](/ActivityDiagram.drawio2.png "Activity Diagram")

