# Documentation
                                  Execution steps
1.	The  JobManagementDirectory folder contains all the libs and config needed for execution of  service.

2.	In the folder you will find following 
        a.	Archieving 
        b.	jobManagement-settings
        c.	Jobs
        d.	Logs
        e.	ArchievingDocumentAPI.jar  (Job for Archiving documents)
        f.	EmailNotification.jar  (Job to send email notifications)
        g.	JobManagementAPI.jar (This is jar which jobs will import to implement job interface)
        h.	JobManagementService.jar( This is executable jar of the project)
3.	In JobManagment-settings update the configurations
        a.	Archieving job settings.
        b.	Email job settings.
        c.	Jobmanagement settings.
        
        This configuration needed for uploading the jobs and executing jobs from the folder. 
        It contains path to Jobs folder.

 4.	Once configuration is done, execute the service JobManagementService.jar
        a.	You will get the following screen.
 5.	Please enter the following details.
        a.	Email Notification Job
            i.	Class path : com.email.notification.impl.EmailNotification
            ii.	Click on the upload button to select the Jar for EmailNotification.
            iii.	The select the time, please update the time as I have not implemented the dynamic time,you can change the minutes ,hours and seconds by clicking on the small buttons as shown in below image.
            iv.	Then click on the schedule now or execute now button to run the job.
 
        b.	Archiving Job (follow Same steps)

            i.	Class path :   com.documents.jobs.Archieve
            ii.	Click on the upload button to select the Jar for ArchievingDocumentAPI.
            iii.	The select the time, please update the time as I have not implemented the dynamic time,you can change the minutes     ,hours and seconds by clicking on the small buttons as shown in below image.

             iv.	Then click on the schedule now or execute now button to run the job.

        c.	We can check the status of the job. 
            i.	We can also check which jobs are in the queue and which got successfully completed or failed. Below are few screenshots.
            ii.	Queued jobs
            iii.	Status check 
            iv.	Success List
 
