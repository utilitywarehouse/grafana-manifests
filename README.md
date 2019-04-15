# Grafana manifests

Grafana manifests used for Kustomize.

`/base` contains base Grafana configuration
`/example` contains example how to use the manifests.

```
.
¿¿¿ base
¿   ¿¿¿ grafana.yaml
¿   ¿¿¿ kustomization.yaml
¿   ¿¿¿ secrets.yaml
¿¿¿ example
¿   ¿¿¿ grafana.yaml
¿   ¿¿¿ kustomization.yaml
¿¿¿ LICENSE
¿¿¿ README.md
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
