# 🔍 Server Monitoring Stack

This project sets up a basic monitoring stack using **Prometheus**, **Grafana**, and **Node Exporter** with **Docker Compose**.

## 🎯 What It Does

- Monitors system metrics using Node Exporter
- Collects data with Prometheus
- Visualizes metrics using Grafana
- Includes a sample Grafana dashboard

## 🧰 Stack

- Prometheus
- Grafana
- Node Exporter
- Docker & Docker Compose

## 📂 Project Structure

```
server-monitoring-stack/
├── docker-compose.yml
├── prometheus/
│   └── prometheus.yml
├── grafana/
│   └── dashboard.json
└── README.md
```

## 🚀 Usage

### 1. Run the stack

```bash
docker-compose up -d
```

### 2. Access services

- Grafana: [http://localhost:3000](http://localhost:3000) (user: admin / pass: admin)
- Prometheus: [http://localhost:9090](http://localhost:9090)
- Node Exporter: [http://localhost:9100](http://localhost:9100)

### 3. Import dashboard

In Grafana:
- Go to **Dashboards > Import**
- Upload `grafana/dashboard.json`

---

Ideal for monitoring dev environments or learning observability tools.
