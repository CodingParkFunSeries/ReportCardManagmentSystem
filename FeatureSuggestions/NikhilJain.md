# Nikhil Jain Feature Suggestions
#### Feel free to correct my mistakes.

## Expected User Base
* Teachers who will enter the data.
* Students or their parents who will visualize and analize that data.
## Proposed Architecture
* We should follow a 3-tier architecture :
  - Frontend (Web App + IOS/Android App)
  - A Web API in between to link Frontend with the Database.
  - Then a Mongo DB database as proposed in problem statement.
* An API is required because:
  - Same REST API could be used in for Web App and phone apps. Or else we have to seperately connect the Web App and phone apps to database. 
  - And if tommorrow we plan to migrate our database let's say from Mongo DB to some other DB, then we have to only change in the API and not in the frontend.
 * Web App could be integrated with Power BI to have an interactive dashboard where we can have several plots for an easy understanding of the student data.
 
 ## Proposed Security Measures
 * In order to secure our application we can have AZURE AD authentication on the top of our frontend.
 * Then we can use features like App to App authentication, securing of connection string etc. only if time allows and is in the scope of problem statement.
 
 **From now on I would be using only Web App. Same could be applied for Android/IOS app.**
 ## Suggested Features
  * On the very first page of Web App, we can have a choice i.e who is the user a teacher or a student.
  * For **_students_**:
    * We can have 4 sections:
      - Profile Section
      - Individual Subject Section
      - Combined Report Section
      - Complaint/Review Section **(Only if time allows)**
    * **Profile Section :** Basic details of student like Name, Roll No, Standard, etc.
    * **Individual Subject Section :** 
      - Name of the teacher who taught that subject.
      - Name of the teacher who worked as the course coordinator for that subject.
      - Marks of all types of assessments like Mid-term, End-term, Sessional.
      - Apart from marks obtained, we can also have what is rank of the student in that particular subject.
      - A total score combining all the assessments i.e. Mid-term + End-term + Sessionals.
      - A list of overall top 10 scorers in that subject (may be in tabular form or in the form of a plot).
    *  **Combined Report Section :**
        - Total scores of all the subjects.
        - A final score combining all the total scores of individual subjects.
        - A final rank of student based on final score.
        - A list of overall top 10 scorers (may be in tabular form or in the form of a plot).
    * **Complaint/Review Section :**
        - A form could me made which the students can fill in case they feel they have obtained less marks.
        - Response of the form would be automatically mailed to the teacher who taught that subject to student and to the course coordinator of that subject.
        
  * For **_teachers_**:
    * We can have 2 sections:
      - Profile Section
      - Individual Subject Section
    * **Profile Section :** Basic details like Name, Teacher ID, Subjects taught etc.
    * **Individual Subject Section :** 
      - Choose the subject.
      - Choose the assessment type - Mid-term, End-term or Sessional.
      - Enter entries of marks where each entry consist of Roll No and Marks obtained.
      - Option of create, edit, delete or update an entry.
      - Option of direct uploading the data in the excel format (**only if we can do**).
      - Option of different analysis like for individual student or overall performance of all students in that subject.
      - A list of overall top 10 scorers in that subject (may be in tabular form or in the form of a plot).
      
    
   * For **_admin_** we have sections to add or delete students, teachers or subjects. 
 
 
  
  
 
 




