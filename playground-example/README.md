# Overview

This docker-compose file runs the WarpStream `playground` command in a docker-compose file and uses the `diagnose-connection` command (running in a separate docker container) to verify that other containers in the compose setup can communicate with the Agent using the Kafka protocol. It also create a new test topic called `docker-compose-test-topic` to make sure everything is working properly.

# How to Run

```bash
docker-compose rm -f
docker-compose pull
```

then:

```bash
docker-compose up
```
