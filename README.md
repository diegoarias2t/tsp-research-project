<p align="center">
<img src=assets/tsp-ipparis.png>
</p>

# TSP Research Project
> Final project designed to implement the different topics learned throughout the course.

## Requirements
1. Python3
2. docker-compose

## Installation

1. Update your system.
```
sudo apt update
```

2. Install docker.
> https://docs.docker.com/engine/install/ubuntu/

Make sure to give the right permissions to your docker.sock folder (we are going to need that later).

```
sudo chmod -R 777 tsp-research-project/
sudo chmod 666 /var/run/docker.sock
```

3. Install docker compose.
> https://docs.docker.com/compose/install/

4. Install jupyter.
> https://www.digitalocean.com/community/tutorials/how-to-set-up-jupyter-notebook-with-python-3-on-ubuntu-18-04

```
sudo apt install swig cmake libopenmpi-dev zlib1g-dev
sudo pip install stable-baselines[mpi]==2.10.2 box2d box2d-kengz
```

5. Install pip requirements.
```
pip install -r requirements.txt
```

6. Implementation of ml_monitor module.
```
pip install -r requirements.txt
```