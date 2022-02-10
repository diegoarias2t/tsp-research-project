<p align="center">
<img src=assets/tsp-ipparis.png>
</p>

# TSP Research Project
> Final project designed to implement the different topics learned throughout the course.

## Requirements
1. Python3
2. Docker engine
3. Docker-compose
4. Jupyter

## Installation

1. Clone this repository
```
sudo git clone https://github.com/diegoarias2t/tsp-research-project
```

2. Update your system.
```
sudo apt update
pip3 install --upgrade pip
```

3. Install docker.
> [`docs.docker.com/engine`](https://docs.docker.com/engine/install/ubuntu/)

Make sure to give the right permissions to your docker.sock folder (we are going to need that later).

```
sudo chmod -R 777 tsp-research-project/
sudo chmod 666 /var/run/docker.sock
```

4. Install docker compose.
> [`docs.docker.com/compose`](https://docs.docker.com/compose/install/)

5. Install jupyter.
```
sudo apt install jupyter-notebook
```

6. Implementation of ml_monitor module.

```
pip3 install .
```

7. Installing the needed dependencies.

```
sudo apt install swig cmake libopenmpi-dev zlib1g-dev
pip3 install -r requirements.txt
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
