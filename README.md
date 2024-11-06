# Install Grafana

[Chart](https://github.com/grafana/helm-charts/blob/main/charts/grafana/README.md)

```sh
helm upgrade --install -n monitoring --create-namespace grafana grafana/grafana -f ./grafana/values.yaml
```

# Install Prometheus

[Chart](https://github.com/prometheus-community/helm-charts)

```
❯ helm upgrade --install -n monitoring --create-namespace prometheus prometheus-community/prometheus -f ./prometheus/values.yaml
```

# Upgrade nginx ingress to enable prom scraping

```
helm upgrade --install -n kube-system nginx-ingress ingress-nginx/ingress-nginx -f ./ingress/values.yaml
```
