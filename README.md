# multi-tenant-metrics-demo

## Install flux

```bash
$ flux install -v v0.33.0 --watch-all-namespaces=false --export > flux-system/flux.yaml
$ kubectl apply -f flux-system/flux.yaml
```

## Init flux

```bash
$ kubectl apply -f flux-system/init.yaml
```

