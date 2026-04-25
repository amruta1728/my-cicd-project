#  CI/CD Project using Jenkins + Ansible + Nginx

##  Overview
This project demonstrates Continuous Delivery using Jenkins and Configuration Management using Ansible.

##  Tools Used
- Jenkins
- Ansible
- Nginx
- AWS EC2

##  Workflow
1. Code pushed to GitHub
2. Jenkins pipeline triggered
3. Ansible deploys app
4. Nginx serves website

##  Access
http://<EC2-IP>

##  Structure
- app/ → static website
- ansible/ → deployment scripts
- Jenkinsfile → pipeline
