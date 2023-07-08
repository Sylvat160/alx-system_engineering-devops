# Project Requirements

## Concepts to Explore
- Load balancer
- Web stack debugging

## Background Context
Two additional servers have been provided for this project:
- gc-[STUDENT_ID]-web-02-XXXXXXXXXX
- gc-[STUDENT_ID]-lb-01-XXXXXXXXXX

The goal of this project is to improve the web stack by introducing redundancy for the web servers. This will increase the capacity to handle more traffic by doubling the number of web servers and enhance the infrastructure's reliability. In case one web server fails, the second server will be available to handle requests.

To accomplish the project requirements, you need to write Bash scripts that automate the necessary configurations on a fresh Ubuntu server.

## Resources
Read or watch the following:

- [Load balancer](https://www.thegeekstuff.com/2016/01/load-balancer-intro/)
- [Introduction to load-balancing and HAproxy](https://www.digitalocean.com/community/tutorials/an-introduction-to-haproxy-and-load-balancing-concepts)
- [HTTP header](https://www.techopedia.com/definition/27178/http-header)
- [Debian/Ubuntu HAProxy packages](https://haproxy.debian.net/#distribution=Ubuntu&release=lunar&version=2.8)
- [Load balacing algorithm](https://community.f5.com/t5/technical-articles/intro-to-load-balancing-for-developers-the-algorithms/ta-p/273759)

## Requirements
General:
- Allowed editors: vi, vim, emacs
- All files should be interpreted on Ubuntu 16.04 LTS
- All files should end with a new line
- Include a mandatory README.md file at the root of the project folder
- All Bash script files must be executable
- All Bash scripts must pass Shellcheck (version 0.3.7) without any errors
- The first line of all Bash scripts should be exactly `#!/usr/bin/env bash`
- The second line of all Bash scripts should be a comment explaining the purpose of the script.