<p align="center">
<img src=assets/tsp-ipparis.png>
</p>

# TSP Research Project
> Final project designed to implement the different topics learned throughout the course. The baseline of the project has been developed on Kubernetes, it implements a MongoDB database structure with a web administrator of the database known as Mongo-express. In my case, I developed two projects, one basic and one advanced. In the advanced project we have the same structure of MongoDB and Mongo-express but in this one a monitoring system is also implemented on Kubernetes using Prometheus and Grafana to obtain metrics on our database.
## Requirements
1. Python3
2. docker-compose

## Installation
> ...
0. sudo apt update

1. Install docker
https://docs.docker.com/engine/install/ubuntu/

make sure to give permissions to your docker.sock folder (going to need that later)
sudo chmod 666 /var/run/docker.sock

1. Install docker compose
https://docs.docker.com/compose/install/

2. Install jupyter
https://www.digitalocean.com/community/tutorials/how-to-set-up-jupyter-notebook-with-python-3-on-ubuntu-18-04