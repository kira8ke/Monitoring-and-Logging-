# Week 3 – DevOps July Challenge: Monitoring & Logging Stack

This project sets up a Monitoring and Logging Stack using:

- **Grafana** (Dashboarding)
- **Prometheus** (Metrics)
- **Loki** (Logs)
- **Promtail** (Log shipping)

Deployed using Docker locally and Fly.io on the cloud.

---

## 🔧 Local Setup (Docker)

### Requirements
- Docker
- Docker Compose

### Run the stack

```bash
git clone https://github.com/kira8ke/monitoring-and-logging.git
cd monitoring-and-logging
docker-compose up -d

