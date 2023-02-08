# ubuntu_server_static_IP

Normally when a Linux distribution is installed, a dynamic IP is assigned to IPv4, for security reasons.
The detail is when that OS is used with App Server, BD, etc. Here enters the issue of Assigning a static IP and with internet access for issues of ambientation
of applications.

Now we have to configure our Ubuntu Server Version 18 | 20 | 22, to assign it a static IP with Internet access:


1.- In the Terminal, wroted:
- ip a

![image](https://user-images.githubusercontent.com/69737708/217601248-103ff601-7c65-46f7-87f5-b62270f8208b.png)

2.- enter in the folde /netplan:
- cd /etc/netplan/
- ls -l
- cp xxx-init.yaml  xxx-init.yaml.bck
- ls -l

![image](https://user-images.githubusercontent.com/69737708/217604135-5465bec4-1287-4a01-9a09-a059d442e7a9.png)


![image](https://user-images.githubusercontent.com/69737708/217603946-28d63aa9-6efc-43e4-932e-8709f2da7d76.png)

3.- remove xxx-init.yaml; and create file static.yaml.
- copy config of https://github.com/firecode16/ubuntu_server_staticIP/blob/master/static.yaml  and paste in the file static.yaml

![image](https://user-images.githubusercontent.com/69737708/217605554-1d624bda-7570-4139-8d05-0d9937ff3c3d.png)

4.- apply changes:

![image](https://user-images.githubusercontent.com/69737708/217605851-8c0b5124-e517-4af5-9061-bb80301fab1a.png)

5.- restart now OS:
- reboot now

6.- check new IP static:
- ip a:

7.- ping internet access:

![image](https://user-images.githubusercontent.com/69737708/217607925-615fe2cb-4cc2-461f-b9c5-8424bba9b1db.png)

8. ready, :)
