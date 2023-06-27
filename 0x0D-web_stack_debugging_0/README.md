# Webstack Debugging Basics

In this project, we will be focusing on the concepts of network basics, Docker, and web stack debugging. The goal is to become proficient in debugging web stacks, which is an essential skill for Full-Stack Software Engineers.

## Background

Web applications and servers often encounter issues and bugs that need to be resolved for them to function correctly. Debugging a web stack involves identifying and fixing these issues to ensure the smooth operation of the application.

In this debugging series, you will be given broken or bugged webstacks. Your task is to manually investigate and identify the root cause of the problem. Once you understand the issue, your ultimate goal is to develop a Bash script that, when executed, will restore the webstack to a working state.

Let's begin with a simple example. Imagine we have a server that requires two specific elements to function properly:

1. A copy of the `/etc/passwd` file in the `/tmp` directory.
2. A file named `/tmp/isworking` containing the string "OK".

Without these two elements, the web application will not work correctly. Our objective is to fix the server by ensuring these requirements are met.

```shell
vagrant@vagrant:~$ docker run -d -ti ubuntu:14.04
Unable to find image 'ubuntu:14.04' locally
14.04: Pulling from library/ubuntu
34667c7e4631: Already exists
d18d76a881a4: Already exists
119c7358fbfc: Already exists
2aaf13f3eff0: Already exists
Digest: sha256:58d0da8bc2f434983c6ca4713b08be00ff5586eb5cdff47bcde4b2e88fd40f88
Status: Downloaded newer image for ubuntu:14.04
76f44c0da25e1fdf6bcd4fbc49f4d7b658aba89684080ea5d6e8a0d832be9ff9
vagrant@vagrant:~$ docker ps
CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES
76f44c0da25e        ubuntu:14.04        "/bin/bash"         13 seconds ago      Up 12 seconds                           infallible_bhabha
vagrant@vagrant:~$ docker exec -ti 76f44c0da25e /bin/bash
root@76f44c0da25e:/# ls /tmp/
root@76f44c0da25e:/# cp /etc/passwd /tmp/
root@76f44c0da25e:/# echo OK > /tmp/isworking
root@76f44c0da25e:/# ls /tmp/
isworking  passwd
root@76f44c0da25e:/#
vagrant@vagrant:~$
```

In the given example, a Docker container running Ubuntu 14.04 is used to simulate the broken server. By executing specific commands inside the container, we can fix the server manually. The answer file should contain the following Bash script:

```shell
sylvain@ubuntu:~$ cat answerfile
#!/usr/bin/env bash
# Fix my server with these magic 2 lines
cp /etc/passwd /tmp/
echo OK > /tmp/isworking
sylvain@ubuntu:~$
```

Keep in mind that you should avoid using interactive software such as emacs or vi within your Bash script. All modifications should be done through the command line, including file editing.

## Installing Docker

For this project, you

 will be provided with a Docker container that you can use to solve the task. If you want to experiment with Docker locally or solve the problem on your own machine or Ubuntu VM, you can follow the installation instructions for your specific operating system:

- [Mac OS](https://docs.docker.com/docker-for-mac/install/)
- [Windows](https://docs.docker.com/docker-for-windows/install/)
- [Ubuntu 14.04](https://docs.docker.com/install/linux/docker-ce/ubuntu/)
- [Ubuntu 16.04](https://docs.docker.com/install/linux/docker-ce/ubuntu/)

## Resources

You can refer to the following commands for additional information:

- `man` or `help`: These commands provide detailed information about other commands and utilities.

## Requirements

- Allowed editors: vi, vim, emacs
- All your files will be interpreted on Ubuntu 14.04 LTS
- All your files should end with a new line
- A `README.md` file at the root of the project folder is mandatory
- All your Bash script files must be executable
- Your Bash scripts must pass Shellcheck without any errors
- Your Bash scripts must run without any errors
- The first line of all your Bash scripts should be `#!/usr/bin/env bash`