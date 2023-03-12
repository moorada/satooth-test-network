# sawtooth-test-network
This repository contains docker stack configurations that allow multiple Hyperledger Sawtooth nodes to be deployed on multiple host machines within a docker swarm. 
## Single node

```
docker stack deploy -c 1node-dev.yaml sawtooth
```


## 5 nodes Poet

```
docker stack deploy -c 5node-poet.yaml sawtooth
```

## 5 nodes PBFT

```
docker stack deploy -c 5node-PBFT.yaml sawtooth
```
Docker volumes are shared only within a host system. So you have to otherwise move all the public keys of the nodes to the root node. (/var/lib/docker/volumes/sawtooth_pbft-shared/_data/validators/)

Grafana web page (http://127.0.0.1:3000), log in as user admin with the password admin.
Portainer web page (http://127.0.0.1:9443/), log in as user admin with the password admin.


