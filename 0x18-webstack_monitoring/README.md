# Monitoring Server

## Background Context
*"You cannot fix or improve what you cannot measure"* is a famous saying in the Tech industry. In the era of data-driven practices, monitoring the performance of our software systems holds significant importance. In this project, we aim to implement a monitoring tool to gather insights into the activities of our servers.

Web stack monitoring can be classified into two primary categories:

1. **Application Monitoring:** This involves collecting data about running software and ensuring it functions as intended.

2. **Server Monitoring:** This focuses on gathering data about virtual or physical servers to prevent overload issues, which could encompass CPU, memory, disk, or network overload.

## Resources
Read or watch the following to enhance your understanding:

- [What is Server Monitoring](https://www.sumologic.com/glossary/server-monitoring/)
- [What is Application Monitoring](https://en.wikipedia.org/wiki/Application_performance_management)
- [System Monitoring by Google](https://sre.google/sre-book/monitoring-distributed-systems/)
- [Nginx Logging and Monitoring](https://docs.nginx.com/nginx/admin-guide/monitoring/logging/)

## Learning Objectives
By the completion of this project, you should be capable of explaining the following concepts to others without needing to consult external sources:

**General**
- The significance of monitoring in system administration
- The two main areas of monitoring: application and server
- The purpose of access logs for a web server (e.g., Nginx)
- The role of error logs for a web server (e.g., Nginx)


## Requirements
**General**
- Permissible text editors: vi, vim, emacs
- Your scripts will be interpreted on Ubuntu 16.04 LTS
- All script files must conclude with a newline character
- A mandatory README.md file at the project's root folder
- All Bash script files must have executable permissions
- Your Bash scripts must pass Shellcheck (version 0.3.7) without errors
- The first line of each Bash script must be exactly `#!/usr/bin/env bash`
- The second line of each Bash script should include a comment explaining the script's purpose