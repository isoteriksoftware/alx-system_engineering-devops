```diff


+ 0x0E. Web stack debugging #1
+ DevOps
! SysAdmin
! Scripting
! Debugging
- By: Sylvain Kalache
 Weight: 1
+ Project will start Jan 18, 2023 5:00 AM, must end by Jan 22, 2023 5:00 AM
 will be released at Jan 20, 2023 7:24 PM
+ An auto review will be launched at the deadline
Concepts
+For this project, we expect you to look at these concepts:

+ Network basics
+ Web stack debugging


- Requirements
- General
+ Allowed editors: vi, vim, emacs
+ All your files will be interpreted on Ubuntu 20.04 LTS
+ All your files should end with a new line
+ A README.md file at the root of the folder of the project is mandatory
+ All your Bash script files must be executable
- Your Bash scripts must pass Shellcheck without any error
- Your Bash scripts must run without error
+ The first line of all your Bash scripts should be exactly #!/usr/bin/env bash
+ The second line of all your Bash scripts should be a comment explaining what is the script doing
+ You are not allowed to use wget
! Tasks
+ 0. Nginx likes port 80
- mandatory
+ Using your debugging skills, find out what’s keeping your Ubuntu container’s Nginx installation from listening on port 80. Feel free to install whatever tool you need, start and destroy as many containers as you need to debug the issue. Then, write a Bash script with the minimum number of commands to automate your fix.

+ Requirements:

+ Nginx must be running, and listening on port 80 of all the server’s active IPv4 IPs
+ Write a Bash script that configures a server to the above requirements
root@966c5664b21f:/# curl 0:80
curl: (7) Failed to connect to 0 port 80: Connection refused
+ root@966c5664b21f:/#
+ root@966c5664b21f:/# ./0-nginx_likes_port_80 > /dev/null 2&>1
+ root@966c5664b21f:/#
+ root@966c5664b21f:/# curl 0:80
- <!DOCTYPE html>
- <html>
- <head>
- <title>Welcome to nginx!</title>
- <style>
    body {
        width: 35em;
        margin: 0 auto;
        font-family: Tahoma, Verdana, Arial, sans-serif;
    }
- </style>
- </head>
- <body>
- <h1>Welcome to nginx!</h1>
- <p>If you see this page, the nginx web server is successfully installed and
working. Further configuration is required.</p>

- <p>For online documentation and support please refer to
- <a href="http://nginx.org/">nginx.org</a>.<br/>
+ Commercial support is available at
- <a href="http://nginx.com/">nginx.com</a>.</p>

- <p><em>Thank you for using nginx.</em></p>
- </body>
- </html>
+ root@966c5664b21f:/#
+ Repo:

+ GitHub repository: alx-system_engineering-devops
+ Directory: 0x0E-web_stack_debugging_1
+ File: 0-nginx_likes_port_80
  
+ Copyright © 2023 ALX, All rights reserved.

! Author:
+ Afolabi John Oluwaseun

```
