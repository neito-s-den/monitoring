# Install Grafana

```sh
helm upgrade --install -n monitoring --create-namespace grafana grafana/grafana -f ./grafana/values.yaml
```
