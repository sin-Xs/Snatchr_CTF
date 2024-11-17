![snatchr_logo](https://i.ibb.co/Scmh4jq/snatchr-logo.png)

Welcome to the **Snatchr CTF**,
This set of challenges was inspired by [**OverTheWire - Bandit**](https://overthewire.org/wargames/bandit/).

**No prior "hacking" knowledge** is required to master the challenges, as long as you **read the help/man pages** (even Google, etc. can be used) for the commands you have trouble with.

This CTF was designed to get to know the general Linux-Environment and maybe even learn something along the way.

I hope you'll have fun! 

## Getting started
#### Import the docker image:
`sudo docker load -i <image.tar>`
<sub>Substitute **\<image.tar\>** with the file that contains the docker image.</sub>

#### Starting the docker container:
`sudo docker run -td -p <desired_port>:22 --name <container_name> <docker_image>`
<sub>**\<desired_port\>** should be a port number that is not used on your system. I recommend **2222**. **\<container_name\>** can be anything. It is used to refer to the docker container later - if needed. And **\<docker_image\>** is the name of the image that was installed by the first command. If you don't know the name (usually: **snatchr_ctf:\<version_number\>**) use the following command: `sudo docker image ls`.</sub>

#### Log into the first level:
`ssh snatchr_0@localhost -p <desired_port>`

> <sub>Here is a short explanation of the ssh-command: `ssh
> <username>@<address> -p <port>` 
> **\<username\>** is the name of the user that you connect to.
> **\<address\>** Usually you will see an IP-address here. In our case **"localhost"** is used. Localhost refers to a special IP-address that connects us to the machine we use the command on.
> **\<port\>** Rarely you need to use "-p \<port\>", because as long as the port is **22**, it is not needed. In our case we use a special
> port (e.g. **2222**).</sub>

<sub>The first time you connect to the container, a message will pop up, asking you for a fingerprint. Accept with **"yes"**. Usually it will only be displayed one time.
The password for the first level is: **snatchr_0**</sub>

## While playing
If you find the password, I recommend you to **take notes**. In case you close and wanna come back to the level, you will need the password again.

After finishing a level, type **"exit"** to close the connection. Then establish another ssh connection for the next user like this: `ssh <username>@localhost -p 2222`, where \<username\> is the next levels user (like **snatchr_15** for level 15).
When asked, use the password you gathered.

At any time, you can receive the password of the user you have access to by typing the command: `cat /etc/snatchr_pw/<username>`, where **\<username\>** is the name of the levels user (e.g **snatchr_1**).

## After playing
... it is recommended to remove the docker container (save the password!):
`sudo docker rm -f <container_name>`
<sub>**\<container_name\>** is the name you have specified in the **"docker run"** command.</sub>

<hr>
<hr>
