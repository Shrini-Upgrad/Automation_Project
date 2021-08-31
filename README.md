# Automation_Project
Upgrad Assignment
This is a read me file to describe the course assignment.

The assignment includes writing a script to configure the Virtual Machine for hosting a web server and later automating some maintainance tasks. 
Hosting Web Server: The first step is to set up a web server on the EC2 instance for hosting a website. It is also important to ensure that the apache2 server is running and it restarts automatically in case the EC2 instance reboots.

Archiving Logs: Daily requests to web servers generate lots of access logs. These log files  serve as an  important tool for troubleshooting.  However, these logs can also result in the servers running out of disk space and can make them stop working. To avoid this, one of the best practices is to create a backup of these logs by compressing the logs directory and archiving it to the s3 bucket (Storage). 

I have to ensure that my script checks for the presence of the inventory.html file in /var/www/html/; if not found, creates it.If an inventory file already exists, the content of the file should not be deleted or overwritten. New content should be only appended in a new line.

My script should create a cron job file in /etc/cron.d/ with the name 'automation' that runs the script /root/<git repository name>/automation.sh every day via the root user.

I have been assigned to write an automation bash script named ‘automation. sh’ to automate all these workflows.
