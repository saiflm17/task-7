# TASK-7 EXPLANATION 

#STEP-1 : am taking a new server with server configurations like server_name, AMI : amazon linux kernel 5.10, instance_type : t2.micro, key_pair, security_group : All Traffic, EBS : 25 GIB .

#STEP-2 : After launching the server and am connecting through SSH .

- Now am creating a New repository in my GitHub and Repository_name : task-7 .

- COMMAND : sudo -i - to change the root user .

- Now am installing docker by using command .

- COMMAND : yum install docker -y - to install the docker .

- COMMAND : systemctl start docker - to start the docker .

- COMMAND : systemctl status docker - to check the status of the docker .

- Now am set-up a netdata monitoring tool by using run via docker .

- COMMAND : docker run -d --name netdata -p 19999:19999 netdata/netdata - this command works on to set-up a netdata monitoring tool .

- http://localhost:19999 - Now am Accessing the netdata monitoring tool .

- After am login-in by using Email-id .

- About NETDATA : Netdata is a lightweight, open-source monitoring tool that gives you real-time insights into the performance of your system and applications .

- Data Collection : Netdata collects metrics from:

- CPU, Memory, Disk, network, Docker Containers .

- Now am creating a New dashboard and Dashboard_name : Deployment - Dashboard .

- and also am  creating some containers by using commands .

- COMMAND : docker run -itd --name cont-01 -p 1111:80 nginx .

- COMMAND : docker run -itd --name cont-02 -p 2222:80 shaikmustafa/dm .

- COMMAND : docker run -itd --name cont-03 -p 3333:80 shaikmustafa/cyclemode .

- so these are the containers am creating in my server to accessing the running metrics .

- And also to check the logs in my server  -  cd /var/log/netdata .

- Now am taking some screenshots of the dashboard and running metrics and also am paste it in my repository . And repository_name : task-7 .


