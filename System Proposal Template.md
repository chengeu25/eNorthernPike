# System Request Document

## Table of Contents

1. System Request
2. Work Plan
3. Feasibility Analysis
   1. Technical Feasibility
   2. Organizational Feasibility
4. Requirements Definition
   1. Functional Requirement
   2. Non-functional Requirement
5. Logical Design
   1. Sequence Diagram
   2. Use Cases
   3. Process Modeling (Data Flow Diagram)
      1. Level 0 Diagram
      2. Level 1 Diagram
      3. Level 2 Diagram
      4. Level 3 Diagram
      5. Level 4 Diagram
      6. Level 5 Diagram
   4. Data Modeling (Entity Relationship Diagram)
   5. Structure Chart Diagram
6. Appendices



## Executive Summary
> A summary of all the essential information in the proposal so that a busy executive can read it quickly and decide what parts of the plan to read in more depth.

## 1. System Request

- **Project Sponsors:** Cheng Eu Sun, Garret Van Dyke, Caleb Rice, Matthew Merlo 
- **Business Requirements**: The Enorthernpike Course Registration System aims to streamline the course registration process by providing a unified, user-friendly platform that integrates functionalities from existing systems like Degreeworks and Ecarps. Key functional requirements include secure user authentication, intuitive course search and registration, degree progress tracking, personalized course recommendations, and robust reporting and analytics capabilities. Non-functional requirements focus on usability, security, scalability, and reliability to ensure a seamless and efficient user experience. Compliance with data protection regulations and integration with existing university systems are also essential considerations.
- **Business Need:** This project has been initiated to create a unified course registry/planner for all Messiah students to create an 8-semester course plan and all necessary course information in one place.
- **Business Value:** Replacing the existing course registration system with a more modern, user-friendly system will provide much value to any university that chooses to use our system. With the information about what classes they need and when they are offered as well as the ability to create an 8-semester plan right at students' fingertips, there will be much fewer confusions that faculty will need to resolve. This will greatly streamline advising. There will also be much less of a need to accomodate students who fail to complete the right courses to earn their degree, as it will be much easier for students to avoid this scenario. Finally, the ease of getting into the right courses and confidence that a student knows what they need to do to graduate can have a major effect on their opinion of the college, so this will help universities retain students and gain more positive feedback in general.
- **Special Issues and Constraints:** Collecting students personal information as it comes to certain classes and times they take them could pose a certain level of conidentiality issue. Deciding the size of the project could be an issue, we need to make sure we add enough features that it will be significantly better than the current system, but not too much that the UI is confusing and too bothersome to learn since students really only use it once a semester. Security may be an issue since all sponsors/group members have taken few cybersecurity classes AKA outsourcing may be a nessecity. 

## 2. Work plan
> The original work plan revised after having completed the analysis phase.
### Gantt Chart
```mermaid 
gantt
    dateFormat  YYYY-MM-DD
    title       YOUR PROJECT TITLE HERE
    excludes    weekends
    %% (`excludes` accepts specific dates in YYYY-MM-DD format, days of the week ("sunday") or "weekends", but not the word "weekdays".)

    section Section A
    Task A.1            :         des1, 2014-01-06,2014-01-08
    Task A.2            :         des2, 2014-01-09, 3d
    Task A.3            :         des3, after des2, 5d
    Task A.4            :         des4, after des3, 5d

    section Section B
    Task B.1            :         des5, 2014-01-07,2014-01-09
    Task B.2            :         des6, 2014-01-10, 7d
    Task B.3            :         des7, after des3, 2d
    Task B.4            :         des8, after des7, 5d

    section Section C
    Task C.1            :         des9, 2014-01-06,2014-01-08
    Task C.2            :         des10, 2014-01-09, 3d
    Task C.3            :         des11, after des2, 5d
    Task C.4            :         des12, after des3, 5d

```

## 3. Feasibility Analysis

### 3.1 Technical Feasibility
Technically, this project is complex but doable. It's really just a standard Model-View-Controller app, with a UI that could be designed with a JavaScript framework like React or Vue, and then we would need a database with several tables and a server-side framework to communicate with it. While there would be some complex design issues in terms of getting the right data in the right place at the right time, these would be worked out in the design phase and at that point it's just coding it which shouldn't be that difficult, especially since we would have a full year to get it working. The main issue with the technical feasibility would be the security. Given that none of the project sponsors are cybersecurity experts, we would need to spend considerable resources looking into this, and since we would be dealing with information protected by FERPA and managed by an actual University, some of which is sensitive, this is not an area that we can afford to do poorly.

### 3.2 Organizational Feasibility
There is a couple of issues in terms of organizational feasibilites, however there are also some organizational feasibilities that are possible for us, so lets start with those. In terms of cost there is really no issue. The financial requirements of the whole system are extremely low. We would most likely need to buy nothing. We would however run into issues in terms of having a member of the current organization keep the system up to date semester over semester. Now onto the issues. The biggest issue is the security risk. Since there is a security risk that we face and we are not apart of the adminsitration there will be some difficulty to get access to information we would need. Also FERPA would make our project difficult since it protects students schedules which is something we would eventually need to deal with. Another problem is since our chosen organization has their own planning system and they don't want to have students getting mixed up with a variety of different planning softwares meaning it would be difficult to have an offical system that the university uses without replacing the current software. Another problem is that our organization is changing how registration works next year (the time we have to create our system) it creates extra difficulties to get the required items that we need from our orginization. Continuing on with the difficulties of obtaining our needed information we may run into some time constraints since we only have a year to get this project done we would need to request information from the registrar/IT early and even then we may not be able to start on certain parts of the project until we get that information meaning that we would have to wait to start certain parts of it.
## 4. Requirements Definition

### 4.1 Functional Requirements:

1. User Authentication
   - Secure login and registration for students, faculty, and staff.
   - Role-based access control to ensure appropriate access levels.

2. Course Planning

   - Intuitive interface for course search and planning.
   - Real-time course availability/offerings status displayed during selection.

3. Degree Progress Tracking

   - Integration with academic records to track degree requirements and progress.
   - Visual representation of completed and remaining courses.

4. Reporting and Analytics

   - Generate reports on course registration, student progress, and system usage.
   - Analytics dashboard for monitoring system performance and user engagement.

5. Course Search

   - Improved ability for course searching by name.

### 4.2 Nonfunctional Requirements:

1. **Operational**

2. **Performance**

3. **Security**

4. **Cultural and political**

## 5. Logical Design

> A set of use cases that illustrate the basic processes that the system needs to support.

### 5.1 Sequence Diagram

```mermaid
sequenceDiagram
   actor J as John
   participant S as System

   S->>J: Enter user name and password
   J-->>S: Types username and password

```

### 5.2 Use Cases
> *Reference Chapter 4*

#### Use Case Name:  Your use case name

> __ID__ :

> __Priority__ :

> __Actor__ :

> __Description__ :

> __Trigger__ :

> __Type__ :

> __Preconditions__ :
>   1. Condition 1
>   2. Condition 2
>   3. ......

| Normal Course:                            | Information for Steps       |
| ----------------------------------------- | --------------------------- |
| 1.0 Finalize Parts Request                |                             |
| 1. Parts room clerk opens the parts . . . | <--- Parts Request record   |
| 2. Parts room clerk verifies . . .        | <--- Shop Work Order Record |

> __Postconditions__ :
>   1. Condition 1
>   2. Condition 2
>   3. ......

| Summary Inputs           | Source           | Summary Outputs         | Destination               |
| ------------------------ | ---------------- | ----------------------- | ------------------------- |
| Final parts verification | Parts room clerk | Parts request record    | Parts room clerk          |
| Date/time completion     | Parts room clerk | Shop work order record  | Shop work order datastore |
|                          |                  | Work Order ready notice | Technician                |
 
### 5.3 Process Model (Data Flow Diagram)
> A set of process models and descriptions for the to‐be system. This may include process models of the current as‐is system that will be replaced.

Level 1:
```mermaid
flowchart TD
d1[[D1: Student/Faculty Login/Program Database]]
d2[[D2: Program Requirements Database]]
d3[[D3: Course Offerings Database]]
d4[[D4: Course Plan Database]]
a1[Student]
a2[Faculty]
1(1\nUpdate Program Requirements)
2(2\nUpdate Course Offerings)
3(3\nView Program Requirements)
4(4\nView/Edit\nRegistration Plan)
5(5\nGet What If Requirements)
7(7\nView Course\nOfferings)
8(8\nLogin)
10(10\nUpdate Student's\nProgram)

a1 --Enter info--> 8 --Check with database--> d1 --Does login exist?--> 8
a2 --Enter info--> 8
8 --Success/Fail --> a1
8 --Success/Fail --> a2
a1 --Go to requirements page--> 3
d2 --Send requirements--> 3
a1 --Go to plan page--> 4 --Update database--> d4
d4 --Read courses-->4
3 --Push updates to database--> d2 --Send requirements to display--> 3 --Display to student--> a1
a1 --Go to offerings page--> 7 --Request offerings--> d3 --Send offerings to display--> 7 --Display to student--> a1
a2 --Submit update request--> 1 --Update in database-->d2
a2 --Submit update request--> 2 --Update in database-->d3
a2 --Confirm update-->10--Update database-->d1
a1--Request What-If and input new requirements-->5--Fetch requirements from database-->d2--Send new requirements-->5--Display to student-->a1
```

### 5.4 Data Model (Entity Relationship Diagram)
> *Reference Chapter 5*

> A set of data models and descriptions for the to‐be system. This may include data models of the as‐is system that will be replaced.

### 5.4 Structure Chart Diagram
> *Reference Chapter 9*

## 6. Appendices
> These contain additional material relevant to the proposal, often used to support the recommended system. This might include results of a questionnaire survey or interviews, industry reports and statistics, etc.
