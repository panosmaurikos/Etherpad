# Etherpad
Etherpad allows you to edit documents collaboratively in real-time, much like a live multi-player editor that runs in your browser. 

**Run etherpad in docker and kubernetes**
##  1. Etherpad Docker 
To run etherpad with docker use the docker-compose.yaml file from Etheroad_Docker folder and run:
~~~
docker compose up -d
~~~
Check if everything is running with the command ```docker ps```, the output must be like this:
~~~
CONTAINER ID   IMAGE                      COMMAND                  CREATED        STATUS                 PORTS                                       NAMES
b60551ce9916   etherpad/etherpad:latest   "docker-entrypoint.s…"   39 hours ago   Up 3 hours (healthy)   0.0.0.0:9001->9001/tcp, :::9001->9001/tcp   etherpad
e69303a83894   mysql:8                    "docker-entrypoint.s…"   39 hours ago   Up 15 hours            3306/tcp, 33060/tcp                         etherpad_mysql
~~~
Also, you can see the etherpad logs with the command ```docker logs <container ID> # b60551ce9916```

## 2. Etherpad Kubernetes

#### Prerequisites
- A running Kubernetes cluster.
- Access to kubectl to manage Kubernetes resources.
- Storage paths available on the nodes to map Persistent Volumes (PVs).

To install etherpad on your kubernetes cluster run:
~~~

~~~

~~~
kubectl apply -f 
~~~

