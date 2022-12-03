<img src="https://user-images.githubusercontent.com/1423657/173144443-fc7ba783-d5bf-47f9-bf59-707693da5ed1.png" width=200px />

# qryn + coroot
Tutorial: qryn + coroot node agent

The [Coroot Node-agent]((https://coroot.com/docs/metric-exporters/node-agent) ) is a Prometheus exporter based on eBPF that gathers comprehensive container metrics.

<img src="https://user-images.githubusercontent.com/1423657/205445466-67a81963-e593-47c3-ad73-8365e68d9e4f.png" width=800px />


## Requirements
- [qryn](https://qryn.dev) or [qryn.cloud](https://qryn.cloud)
- [grafana](https://grafana.com)

## Usage
The provided `docker-compose` will spin up a coroot-agent and vector scraper pointed at your qryn instance
```
export QRYN_URL=http://qryn:3100/prom/remote/write
docker-compose up -d
```

### Coroot UI
#### Configuration
On your first usage, create a new project and point it at your **qryn** API endpoint

<img src="https://user-images.githubusercontent.com/1423657/205444113-b52ddc6c-c8a1-4e38-b6ed-2e8cc26bd5ed.png" width=600px />

#### Usage
Once metrics are being collected they will automatically display in the coroot user interface

<!-- 
![image](https://user-images.githubusercontent.com/1423657/205444050-21fb7a10-d0d0-4cf1-85fb-98ba3141ec71.png) 
<img src="https://user-images.githubusercontent.com/1423657/205444493-4b3ec904-ff72-424a-b272-9a9e2503594a.gif" width=600px />
-->

<img src="https://user-images.githubusercontent.com/194465/195115881-babd5bd0-8c2b-4718-9cc6-e6dfb5a20c00.gif" width=800px />
