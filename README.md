# 🚀 Grafana + Prometheus Demo

Tento repozitář obsahuje **jednoduché demo** pro monitoring stack:  
**Prometheus** jako time-series databáze + **Grafana** jako vizualizační nástroj.

<pre>

grafana-prometheus-demo/
├── docker-compose.yml
├── prometheus/
│   └── prometheus.yml
├── grafana/
│   └── dashboards/
│       └── example-dashboard.json
├── README.md

</pre>



---

## 📂 Složky

- `docker-compose.yml` – spouští Prometheus a Grafanu.
- `prometheus/prometheus.yml` – konfigurace scrape.
- `grafana/dashboards/` – ukázkový dashboard (JSON).

---

## ⚙️ Jak spustit

1️⃣ Klonuj repozitář:
```bash
git clone <tvůj-git-repo-url>
cd grafana-prometheus-demo
```

2️⃣ Spusť stack:
```bash
docker-compose up -d
```

3️⃣ Otevři:
```bash
    Prometheus: http://localhost:9090

    Grafana: http://localhost:3000
```

4️⃣ Přihlas se do Grafany:
```bash
Username: admin
Password: admin
```

5️⃣ Přidej Prometheus datasource (http://prometheus:9090) a importuj dashboard z grafana/dashboards/.
