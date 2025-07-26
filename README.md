Week 3 – Monitoring and Logging Stack with Prometheus, Grafana, Loki & Promtail

🚀 Overview
This project is part of the July DevOps Challenge (Week 3) where the goal was to implement a complete Monitoring and Logging Stack using open-source tools that provide metrics collection, visualization, and log aggregation.

🔹 Prometheus - Time-series metrics collection
🔹 Grafana - Visualization & dashboards
🔹 Loki - Log aggregation
🔹 Promtail - Log shipping agent for Loki

All services are containerized and orchestrated using Docker Compose, then deployed to Fly.io for public access.

🧰 Technologies Used
Tool	Purpose
Prometheus	Scrapes and stores metrics from exporters
Grafana	Dashboarding and metric/log visualization
Loki	Centralized logging system (from Grafana Labs)
Promtail	Ships local logs to Loki
Docker Compose	Local orchestration of services
Fly.io	Lightweight cloud platform for deployment

🛠️ Local Setup Instructions
Clone the repo

cd devops-july-week3

Run the stack

docker-compose up -d

Access Grafana

-URL: http://localhost:3000

-Login: admin

-Password: admin

Configure Data Sources in Grafana

-Go to Configuration → Data Sources

  --Add Prometheus:
  
URL: http://prometheus:9090

  --Add Loki:
  
URL: http://loki:3100

☁️ Hosting on Fly.io

To deploy on Fly.io:

-flyctl launch

-flyctl deploy

Ensure your fly.toml and Docker Compose configuration are Fly.io compatible.

📊 Dashboards

Sample dashboards included:

-System Metrics (CPU, memory, etc.) via Prometheus

-Log Streams from Docker containers via Loki

📌 Key Learnings

✅ Setting up real-time observability stacks

✅ Working with Docker Compose for multi-service orchestration

✅ Deploying containerized monitoring systems on Fly.io

✅ Understanding the synergy between logs and metrics

✅ Hands-on Grafana dashboard setup and alerting

🌐 Live Preview

🔗 Hosted Version on Fly.io
