# multi-tenant-metrics-demo

This gitops project showcases:

- Kubernetes
- Prometheus
- Grafana
- GitOps
- Multi-tenancy

## Install flux

```bash
$ flux install -v v0.41.2 --watch-all-namespaces=false --export > cluster/components/flux-system/flux.yaml
$ kubectl apply -f cluster/components/flux-system/flux.yaml
```

## Init flux

```bash
$ kubectl apply -f cluster/components/flux-system/seed.yaml
```

## Colima

node-exporter seems to be not working in colima

## Todo

- Network Policies
- Tenant template? (Helm chart?)
- Better docs

# License

None