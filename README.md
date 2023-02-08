# ubuntu_server_static_IP

Normally when a Linux distribution is installed, a dynamic IP is assigned to IPv4, for security reasons.
The detail is when that OS is used with App Server, BD, etc. Here enters the issue of Assigning a static IP and with internet access for issues of ambientation
of applications.

Now we have to configure our Ubuntu Server Version 18 | 20 | 22, to assign it a static IP with Internet access:


1.- In the Terminal, wroted:
- ip a

![image](https://user-images.githubusercontent.com/69737708/217601248-103ff601-7c65-46f7-87f5-b62270f8208b.png)

2.- enter in the folde /netpla:
- cd /etc/netplan/
- ls -l
- cp xxx-init.yaml  xxx-init.yaml.bck
- ls -l

![image](https://user-images.githubusercontent.com/69737708/217604135-5465bec4-1287-4a01-9a09-a059d442e7a9.png)


![image](https://user-images.githubusercontent.com/69737708/217603946-28d63aa9-6efc-43e4-932e-8709f2da7d76.png)

3.- 


