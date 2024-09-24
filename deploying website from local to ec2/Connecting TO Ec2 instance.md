command use to connect ec2 with your machine

> ssh -i testmechine.pem ubuntu@99.79.64.141

ssh -i path of .pem file then ec2 instance ipv4 public


change project to zip file using command

> zip -g file name

secure coping from local to ec2 instance or any other location

> scp  scp -i /home/ibrar-ali/Downloads/testmechine.pem vitalsteer-web.zip ubuntu@99.79.64.141:/home/ubuntu/
