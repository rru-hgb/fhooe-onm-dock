# Installation of fhooe-onm-dock

## Get repo

Install it in any path on your computer.
Open Powershell (PS) or other Terminal (prompt may be different in this case).

```shell
git clone https://github.com/rru-hgb/fhooe-onm-dock.git
```

## Docker

```shell
cd fhooe-onm-dock
docker compose up -d
```
Access mongodb via commandline in container
```shell
docker exec -it onmdb /bin/bash -c "mongosh"
```
Access node container
```shell
docker exec -it onm /bin/bash
```
Subfolder node/ is mapped to /home/node in node container. 


### External Ports

Access them via localhost:nnnn
```
22222 MongoDB 
9999 Mongo-Express
3333 Express
5555 Vite Dev Server
```

### Internal Mongo Connection:

mongo:27017