# Background Context

In this project, you have been given access to an Ubuntu server located in a remote datacenter. To connect to the server, you will use SSH (Secure Shell) with an RSA key instead of a password. The server has already been configured with the public key you generated in a previous project, which can be found in your intranet profile.

To connect to the server, you can retrieve the necessary information from the "My Servers" section in the intranet. Each line contains the IP address and username that should be used for SSH connection.

Note: The server is running Ubuntu 20.04 LTS.

## Resources

To complete this project, you should read or watch the following resources:

- [What is a (physical) server - text](https://en.wikipedia.org/wiki/Server_%28computing%29#Hardware_requirement)
- [What is a (physical) server - video](https://www.youtube.com/watch?v=B1ANfsDyjeA)
- [SSH essentials](https://www.digitalocean.com/community/tutorials/ssh-essentials-working-with-ssh-servers-clients-and-keys)
- [SSH Config File](https://www.ssh.com/academy/ssh/config)
- [Public Key Authentication for SSH](https://www.ssh.com/academy/ssh/public-key-authentication)
- [How Secure Shell Works](https://www.youtube.com/watch?v=ORcvSkgdA58)
- [SSH Crash Course](https://www.youtube.com/watch?v=hQWRp-FdTpc) (Long, but highly informative. Watch this if configuring SSH is still confusing. It may be helpful to watch at x1.25 speed or above.)
- [Understanding the SSH Encryption and Connection Process](https://www.digitalocean.com/community/tutorials/understanding-the-ssh-encryption-and-connection-process)
- [Secure Shell Wiki](https://en.wikipedia.org/wiki/Secure_Shell)
- [IETF RFC 4251](https://www.ietf.org/rfc/rfc4251.txt) (Description of the SSH Protocol)
- [Internet Engineering Task Force](https://en.wikipedia.org/wiki/Internet_Engineering_Task_Force)
- [Request for Comments](https://en.wikipedia.org/wiki/Request_for_Comments)

You may also refer to the following manual or help pages:

- `ssh`
- `ssh-keygen`
- `env`

## Learning Objectives

By the end of this project, you should be able to explain the following concepts without using external resources:

1. General understanding of what a server is.
2. The typical location of servers.
3. Definition and functionality of SSH.
4. The process of creating an SSH RSA key pair.
5. How to connect to a remote host using an SSH RSA key pair.
6. The advantages of using `#!/usr/bin/env bash` instead of `/bin/bash`.

## Copyright - Plagiarism

Remember that you must come up with your own solutions to the tasks in this project to fulfill the learning objectives. Copying and pasting someone else's work or publishing the content of this project is strictly prohibited. Any form of plagiarism will result in removal from the program.

Make sure to include a `README.md` file at the root of the project folder, and all your Bash script files should be executable. Additionally, the first line of each Bash script should be `#!/usr/bin/env bash`, and the second line should be a comment explaining what the script does.