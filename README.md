# multi-tenant-metrics-demo

## Install flux

```bash
$ flux install -v v0.33.0 --watch-all-namespaces=false --export > cluster/components/flux-system/flux.yaml
$ kubectl apply -f cluster/components/flux-system/flux.yaml
```

## Init flux

```bash
$ kubectl apply -f cluster/components/flux-system/seed.yaml
```

## Colima

node-exporter seems to be not working in colima
