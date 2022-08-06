# Home assistant setup
With:
- DRMS integration (for reading my smart meter)
- Influxdb (for storing de DRMS sensory data)
- Grafana (for visualizing the DRMS sensory data)


Works on my raspberry pi 

## Install
```bash
docker compose up -d
```

## Home assistant

## InfluxDB
```bash
# login into running container
docker exec -it influxdb /bin/bash

# open the influx CLI
influx -precision rfc3339

# create a database
CREATE DATABASE home_assistant
```

## Grafana
default username:password = admin:admin