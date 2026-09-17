# Multi-Container Voting App with Prometheus & Grafana Monitoring

A complete cloud-native microservices application (Voting App) integrated with real-time performance monitoring using **Prometheus** and **Grafana**.

---

## 🏗️ Project Architecture

This application consists of multiple distributed components:
* **Vote (Python):** Front-end web app that lets users vote between two options.
* **Redis (Queue):** In-memory queue that collects new votes.
* **Worker (.NET):** Background worker that consumes votes and stores them in the database.
* **Postgres (Database):** Persistent relational database stored for votes data.
* **Result (Node.js):** Front-end web app that shows the results of the voting in real-time.
* **Prometheus:** Scrapes application and container metrics.
* **Grafana:** Visualizes metrics through custom dashboards.
  
