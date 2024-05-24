# Mongodb task

Design database for Zen class programme

1. zenclassdb database is created which contains collections users,tasks,topics,mentors,company_drive,attendance and codekata.

2. The data for the collections are entered manually according to the task need.

3. Find all the topics and tasks which are thought in the month of October
   
        =>for this tasks and topics data are combined in topicandtask collection and the collection data which satisty the above requirement is displayed(which was achieved by using operators).

4. Find all the company drives which appeared between 15 oct-2020 and 31-oct-2020

        =>here, the collection data is aggregated using match based on the given condition.

5.Find all the company drives and students who are appeared for the placement.

        =>for this the company_drive collection is linked to user collection and the commondata required are stored under placement.The users who attendent the drive are displayed along with the company attended.

6.Find the number of problems solved by the user in codekata

        =>the users and codekata collections are merged and the number of problems solved by the user is displayed using aggregation.

7.Find all the mentors with who has the mentee's count more than 15

        =>the users and mentor collections are merged and aggregated based on the requirement(the mentors with mentee count more than 15) and displayed.

8.Find the number of users who are absent and task is not submitted  between 15 oct-2020 and 31-oct-2020

        =>here, three collections user,topic and tasks are merged and aggregated based on the requirement(users who are absent and task is not submitted  between 15 oct-2020 and 31-oct-2020)
