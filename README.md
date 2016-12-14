# Learning Docker

These are the trials, tribulations, and experiments I go through in the process of learning docker.  The items and documentation in this repo will change many times.

## Goal set 1

- Create a VM with docker in it
- Create a docker container with MySQL
- Create a another docker container
- Create a docker container provisioned to run a php hello world application.  
- Create a docker container that uses rails test apps
- Create a docker container that talks to a the MySQL database

## Goal set 2

- Create a VM with Docker
- Create a docker container for fedora
- Create a docker container for solr
- Create a docker container for a hydra app
- Use these containers as a working Hydra Stack
- Try this with actual data
- Modify from there  


## HOST MACHINE

Should be barebones, only docker and basic provisioning should be added.
All of the provisioning should be done in individual containers through the use of dockerfiles and building with docker.  

## First Docker Container

- Use Docker Hub to locate a base docker image `https://hub.docker.com/_/centos/`
  - `docker pull centos` to pull the latest centos box
  - verify that the docker image is now on your machine by running `docker images`
  - run the docker image by `docker run centos`

- Use this to Create another docker image
  - `docker build /vagrant/FirstDockerContainer`
