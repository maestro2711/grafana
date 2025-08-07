# monitoring-tools
liste des outils pour le monitoring des applications
## configure driver docker
- first. identify the Processor
```sh
dpkg --print-architecture
```

- install driver
```sh
docker plugin install grafana/loki-docker-driver:3.3.2-amd64 --alias loki --grant-all-permissions

```
# after install, restart docker
```sh
systemctl restart docker
```