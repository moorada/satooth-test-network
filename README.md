# sawtooth-test-network

## Single node

```
docker stack deploy -c 1node-dev.yaml sawtooth
```

On the Grafana web page (http://127.0.0.1:3000), log in as user admin with the password admin.


## 4 nodes

```
docker stack deploy -c 4node-poet.yaml sawtooth
```

On the Grafana web page (http://127.0.0.1:3000), log in as user admin with the password admin.


