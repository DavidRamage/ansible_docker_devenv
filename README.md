# ansible_docker_devenv
Creates a development environment with Nginx and a Posgres DB using Docker Compose.
## dependencies
This little demo requires that you have Docker Compose installed on your workstation.  It also requires that you have the community Posgres and Docker Ansible modules installed.
## File details
### deploy-devenv.yml
This is the main playbook which launches the others.
### vars.yml
This file contains a minimal set of variables needed to build everything
### roles/deploy_containers/tasks/main.yml
Tasks needed to get the containers up and running
### roles/db_structure/tasks/main.yml
Tasks needed to build the database used for app development and the tables contained therein.
### roles/db_users/tasks/main.yml
Tasks needed to create the users for the database.
### docker/docker-compose.yml
The instructions Docker needs to launch the database and web servers.
