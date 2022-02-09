<p align="center">
<img src=assets/tsp-ipparis.png>
</p>

# TSP Research Project
> Final project designed to implement the different topics learned throughout the course.

## Requirements
1. Python3
2. Docker engine
3. Docker-compose

## Installation

0. Clone this repository
```
sudo git clone https://github.com/diegoarias2t/tsp-research-project
```

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

sudo apt install jupyter-notebook

5. Implementation of ml_monitor module.

```
sudo pip3 install .
```

6. Install pip requirements.

```
sudo apt install swig cmake libopenmpi-dev zlib1g-dev
sudo pip3 install stable-baselines[mpi]==2.10.2 box2d box2d-kengz
sudo pip3 install daiquiri gputil psutil numpy pydrive gym==0.20.0 matplotlib prometheus_client tensorflow==1.15.2 pyyaml
```

## Running the project
1. Starting our docker environment.
```
cd docker/
sudo docker-compose up
```
2. Initializing ml_monitor to send data to our pushgateway.
```
python3
```
```
>>> import ml_monitor
>>> ml_monitor.control.start()
```
3. Execute your Jupyter Notebook and start sending metrics.
```
jupyter notebook
```
