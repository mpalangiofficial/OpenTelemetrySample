# OpenTelemetrySample
## Prometheus-config.yaml
```yaml
global:
  scrape_interval: 15s
  evaluation_interval: 15s

scrape_configs:
  - job_name: "Metrics.NET"

    static_configs:
      - targets: ["host.docker.internal:5169"]
```
## docker Prometheus
``` docker
docker run -d -p 9090:9090 -v D:\Practices\dotnetmetric_examples\prometheus:/etc/prometheus --name prometheus prom/prometheus
```

`#promethes`,`#prometheus config file`,`#prometheus.yml`,`#opentelemetry`,`#instrument`,`#metric`