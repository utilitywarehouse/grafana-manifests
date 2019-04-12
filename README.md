# Grafana manifests

Grafana manifests used for Kustomize.

`/base` contains base Grafana configuration
`/dev-aws` contains configuration specific for aws dev.

```
tree
.
??? LICENSE
??? README.md
??? base
?   ??? grafana.yaml
?   ??? kustomization.yaml
?   ??? secrets.yaml
??? dev-aws
?   ??? grafana.yaml
?   ??? kustomization.yaml
??? dev-gcp

3 directories, 7 files
```

## Example

Check out `kustomization.yaml` in `dev-aws` directory. 

You can build example with:

```
kustomize build dev-aws
```

## Requires

- https://github.com/kubernetes-sigs/kustomize

```
go get -u sigs.k8s.io/kustomize
```
