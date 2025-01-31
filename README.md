# 1-Website-docker-hosting
Putting Webiste in Dacker Caontainer then Hosting



In this I am Putting  static Webiste in Docker Cantainer and then running apache server and hosting it live by copying instance public ip and running in browser 

Following are the Steps to get Starting:

Requirements: AWS Management Console 


steps:
1) Go to Managemnt Console  Go to Ec2 -> give name -> select os (amzon linux free) ->  create ne key pair -> click on launch instance ->  instnace created sucesfully
   ->  now go to AWS Cloud shell -> put su command ->  yum update -y -> yum install docker -y -> docker --version or yum install -y vim nano(if got error st vi) -> service docker start  ->  service docker status ->  docker search amazonlinux ->  docker pull amazonlinux ->  docker images -> docker ruun -td ---name webserver -p 80:80 amzonlinux -> docker port webserver -> docker exec -it webserver /bin/bash ->  yum update -y -> yum install httpd -y -> cd var/www/html -> /usr/sbin/httpd (vi or nano)/root/.bashrc -> vi index.html -> write your code in index.html file -> then copy your aws instance public ip and put into browser and ssee website live 


if Encounter Any Error Visit GeeksforGeeks Documentation.

