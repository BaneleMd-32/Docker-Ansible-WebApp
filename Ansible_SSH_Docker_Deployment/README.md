# Dockerized Web Application Managed by Ansible

This project is a simple demo I built to practice automated deployments.  
It shows how you can use **Docker** together with **Ansible** to spin up a containerized web app without having to manually configure everything yourself.

The idea is pretty straightforward: Ansible connects to a remote server over SSH, writes out a Dockerfile, builds an image, and then runs a container that serves a static HTML page. It’s a neat way to see how infrastructure automation works in practice.

---

## Features

- Ansible playbook automatically creates a Dockerfile on the remote host
- Builds a Docker image and runs a container
- The container serves a basic HTML page that explains the deployment
- Secure management of remote hosts via SSH
- Inventory file makes it easy to add multiple webservers
- Deployment is fully automated and repeatable (no manual steps needed)

---

## Project Structure

Right now the project is kept simple:
- **Playbooks**: Handle the automation steps (create Dockerfile, build image, run container)
- **Inventory**: Defines which servers to connect to
- **HTML page**: A static file served inside the container

---

## Notes

I made this project mainly for learning purposes, so it’s not production‑ready.  
But it’s a good starting point if you’re new to Ansible or Docker and want to see how they can work together. Feel free to clone it, tweak the playbooks, and experiment with your own containers.