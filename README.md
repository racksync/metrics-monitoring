# Monitoring Stack with Docker Compose

This repository contains a Docker Compose setup for a simple monitoring stack, which includes [Grafana](https://grafana.com/), [Prometheus](https://prometheus.io/), and [Node Exporter](https://github.com/prometheus/node_exporter).

## Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Configuration

Clone this repository and navigate into the directory:

```sh
git clone https://github.com/racksync/metrics-monitoring
cd metrics-monitoring

```

Configure the Grafana admin password by editing the .env file:

```GF_SECURITY_ADMIN_PASSWORD=[YourSecurePassword]```

### Start the stack

Start the stack in the background using Docker Compose:

```sh
docker-compose up -d
```

### Access the stack

Access the stack via Grafana at [http://localhost:3000](http://localhost:3000). Log in with the username `admin` and the password you configured in the .env file.


### Add Prometheus as a data source in Grafana

1. Navigate to "Settings" > "Data Sources" > "Add data source".
2. Choose "Prometheus".
3. Set the HTTP URL to `http://prometheus:9090`.
4. Click "Save & Test".


### Create or Import Dashboards

To create a new dashboard, use the Grafana UI to build your visualizations.

To import a pre-made dashboard, navigate to "Dashboards" > "Manage" > "Import" and provide the JSON or Grafana.com ID.

## Notes

- Security: Ensure to secure your deployment, especially if it's used in a production environment.
- Data Persistence: For long-term usage, consider configuring volumes to persist data across restarts and container recreation.

### Automation Training

- [Services & Products](http://racksync.com)
- [Automation Course](https://facebook.com/racksync)

### Community

- [Home Automation Thailand](https://www.facebook.com/groups/hathailand)
- [Home Automation Marketplace](https://www.facebook.com/groups/hatmarketplace)
- [Home Automation Thailand Discord](https://discord.gg/Wc5CwnWkp4)

## [RACKSYNC CO., LTD.](https://racksync.com)

We helps our customers to create life easier across the border of entire technology stack with household and business solutions. We modernize life with Information Technology, Optimize and collect data to make everything possible, secure & trusty
\
\
RACKSYNC COMPANY LIMITED \
Suratthani, Thailand \
Email : devops@racksync.com \
Tel : +66 85 880 8885

[![Home Automation Thailand Discord](https://img.shields.io/discord/986181205504438345?style=for-the-badge)](https://discord.gg/Wc5CwnWkp4) [![Github](https://img.shields.io/github/followers/racksync?style=for-the-badge)](https://github.com/racksync)
[![WebsiteStatus](https://img.shields.io/website?down_color=grey&down_message=Offline&style=for-the-badge&up_color=green&up_message=Online&url=https%3A%2F%2Fracksync.com)](https://racksync.com)
