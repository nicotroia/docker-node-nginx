# Dockerized node + nginx app

This sample project includes a basic node (express) app, spawned on 2 instances, load-balanced via nginx. Refresh the page to see round-robin in action with a custom message from each container.

## Installation

* Install [Docker](https://docs.docker.com/docker-for-mac/install/)

## Create machine (optional)

* Run `docker-machine create -d virtualbox my-project` to create a machine on virtualbox
* View the [machine docs](https://docs.docker.com/v17.12/machine/drivers/) for specific commands for other drivers such as digitalocean or aws
* Run `eval $(docker-machine env my-project)` to run commands against the new machine

## Start

* Run `docker-compose -f docker-compose.yml up` to start the containers

## Connecting

* (optional) Run `docker-machine ip my-project` to find the machine ip
* Point your browser to the ip (localhost:80) or use curl
