# Symptom-Checker
This is a Symptom Checker Application

Application was developed using the Python's Flask framework

After the application was developed, it was deployed on AWS EC2 using nginx and uwsgi servers

Elastic Load Balancers (ELB) were attached to the EC2 on which application was deployed

Load tests were performed on this application and it showed that when no of requests increased to more than 90.000 then a new
EC2 instance was started on its own by the ELB and thus the applicaiton now served from two EC2 instances.

The application served data stored in a json file which resided on AWS S3 bucket.
