# Project 1 Expense Reimbursement API (SRE)
## Project Description
The Employee Reimbursement System (ERS) is a REST API that helps manage the process of reimbursing employees for expenses. Employees can be created and edited via the API. Expenses for employees can be added and updated to pending and approved. The application is a docker-compose project on a remote compute instance, hosted on the AWS Cloud Platform. Monitoring is also implemented, using Prometheus and Grafana.
## Technologies Used
- Java 8
- Javalin (Jetty Server)
- PostgreSQL
- DBeaver
- Postman, 
- Amazon Web Services
- EC2
- RDS
- Prometheus
- Grafana
- Docker
## Features
- Login as Employee of Financial Manager
- Employee can send requests for reimbursement
- Employee can look at list of their own pending or past requests
- Financial Manager can approve/deny request
- Financial Manager can look at list of all pending or past requests
## Getting Started
1. Set up AWS account and EC2 instance
2. Make and download ssh key file
3. Open Gitbash to ssh key file location
4. Enter command to connect to EC2 instance: ssh -i "<SSHkey.pem>" \<EC2 Public DNS\>
5. Once in EC2 instance, set up the environment with these featues:
  - Install Java https://docs.aws.amazon.com/corretto/latest/corretto-8-ug/amazon-linux-install.html
  - Install Git https://cloudaffaire.com/how-to-install-git-in-aws-ec2-instance/
  - Install Docker https://docs.aws.amazon.com/AmazonECS/latest/developerguide/create-container-image.html
6. Enter the following commands:
  - sudo yum update -y
  - sudo yum install maven
  - mkdir gitdir
  - cd gitdir/
  - git clone git@github.com:2205JavaSRE/expense-reimbursement-system-cmhill5.git
  - cd expense-reimbursement-system-cmhill5/
  - docker build -t chance562/p1-ers-api:new
  - docker-compose up
7. View deployed project at "\<EC2 Public DNS\>:7465/"
8. View Prometheus at "\<EC2 Public DNS\>:9090/"
9. View Grafana at "\<EC2 Public DNS\>:8000/"
## Usage
On Postman, use this address "\<EC2 Public DNS\>:7465/" allong with these 
## License
  This project uses the following license:
