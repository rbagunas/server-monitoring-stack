# 🔍 Server Monitoring Stack with Ansible

This project sets up a monitoring stack using **Prometheus**, **Node Exporter**, and **Grafana** using **Ansible** for automation.

## 🎯 What It Does

- Installs and configures Prometheus
- Deploys Node Exporter on target nodes
- Sets up Grafana with a sample dashboard
- Automates the process using Ansible

## 🧰 Stack

- Prometheus
- Grafana
- Node Exporter
- Ansible

## 📂 Project Structure

```
server-monitoring-stack/
├── ansible/
│   ├── inventory
│   ├── prometheus.yml
│   ├── grafana.yml
│   ├── node_exporter.yml
│   └── files/
│       └── dashboard.json
└── README.md
```

## 🚀 Usage

### 1. Update inventory file

Add your target server(s) in `ansible/inventory`

```
[monitoring]
your.server.ip ansible_user=root
```

### 2. Run playbooks

```bash
cd ansible

ansible-playbook -i inventory prometheus.yml
ansible-playbook -i inventory node_exporter.yml
ansible-playbook -i inventory grafana.yml
```

Then access Grafana on port `:3000` of your server.

---

> Perfect for automating your monitoring setup on fresh servers.

