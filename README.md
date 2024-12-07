# Dozzle-Docker-Project
## Introduction
Dozzle is a lightweight, real-time log viewer specifically designed for Docker containers. It provides an intuitive and user-friendly web interface to view and monitor Docker container logs without the need for complex setup or manual log file management.
As a single binary application, Dozzle focuses on simplicity and performance, making it an ideal choice for developers, administrators, and IT professionals who need to monitor logs in real-time. It requires no additional configuration, allowing users to access logs instantly by running it as a Docker container.


Some key features of Dozzle include:
+ Real-Time Log Monitoring: View logs from running Docker containers in real-time.
+ Web-Based Interface: Access logs through a clean, responsive web interface accessible from any browser.
+ Zero Configuration: Automatically detects running containers and displays their logs.
+ Lightweight: Minimal resource usage, ensuring it runs efficiently even on resource-constrained systems.
+ Customizable: Offers options to filter logs and adjust settings based on your needs.

## Pre-requisites

1. A system with Docker installed and configured. 

2. Basic knowledge of command-line tools.

## Steps
### Pulling the Dozzle Docker Image

docker pull amir20/dozzle

### Running Dozzle in a Container

docker run --name dozzle -d --volume=/var/run/docker.sock:/var/run/docker.sock:ro -p 8888:8080 amir20/dozzle:latest

## Video


https://github.com/user-attachments/assets/1db7582a-19ed-49c4-803c-5b0eeb5c3357



## Conclusion
This will deploy Dozzle as a Docker container and gain real-time insights into your Docker container logs. This setup ensures a lightweight, efficient, and easily maintainable solution for log monitoring.

Dozzle can save time and effort by eliminating the need to manually access log files or execute Docker commands repeatedly. Its web-based interface simplifies log monitoring, making it accessible to both developers and system administrators.

Deploying Dozzle using Docker allows for seamless integration into existing workflows and provides the flexibility to scale as needed. 
