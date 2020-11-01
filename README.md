# Ansible-Sample-Application-Deployment
This repository will contain sample code to deploy the sample application on linux instance

Directory Structure
configs - contain environment specific variable

inventories - contains inventory file for each environment

groups_vars - contains common variables across environments

roles - This will have subfolders like java,tomcat

a) tomcat - this folder will have files related to the installation of tomcat

     - files (This will contain files which you want to copy to to your destination servers)

     - handlers ( This is used to start/stop the services)

     - templates (This will contain template files)

     - tasks ( playbook to install the software)
b) add_devops_user - This folder will have files related to the setup of initial user

main.yml - This is the main file which will execute roles in the playbook

