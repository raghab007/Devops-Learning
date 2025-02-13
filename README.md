# Day1 of DEVOPS

> windows/System32/etc/host 
We can open this file through note pad to edit the local DNS addresses

## AWS
Steps to setup EC2 instance in aws
1. select EC2 (Elastic compute version 2)
2. give virtual machine a name 
3. selecct the os
4. select the os version
5. select the instance type
6. create a new key pair (public, private) which is used to ssh into the remote machine
7. add a new security group (Its decides which port number is available or accessible and which device (ip address) can send the request )
    **Security Groups act as a virtual firewall that controls inbound and outbound traffic to your EC2 instances. You can configure a security group to specify which IP addresses or IP ranges are allowed to send requests to your EC2 instance, including allowing or restricting SSH access.**


To acces the remote vm thorugh SSH
ssh -i private-key-file-name username@ipaddress 
Enter the private-key passwrod (if it has been set)
So if you want to deploy the node js into the vm follow theses Steps
install nodejs in the vm using node version manager
clone the repo into the vm


## nginx
> nginx is a tool used for the reverse proxy. Reverse proxy means sending the request to the server based on where the request comes from.
We can run different process of node js on the same process and client doesnot need to specify the port number while sending the requests

Steps to install the nginx in ubuntu 
1. sudo apt update (if needed)
2. sudo apt install nginx
3. change nginx configuration
4. sudo vi /etc/nginx/nginx.cong (configure this file)