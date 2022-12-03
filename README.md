# qryn + coroot
Tutorial: qryn + coroot node agent

The [Coroot Node-agent]((https://coroot.com/docs/metric-exporters/node-agent) ) is a Prometheus exporter based on eBPF that gathers comprehensive container metrics.

![image](https://user-images.githubusercontent.com/1423657/205441435-7e69e252-b47a-45bf-86a7-1552b3731db6.png)

## Requirements
- qryn
- grafana

## Usage
The provided compose will spin up a coroot-agent and vector scraper pointed at your qryn instance
```
export QRYN_URL=http://qryn:3100/prom/remote/write
docker-compose up -d
```

