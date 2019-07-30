# Grafana manifests

Grafana manifests used for Kustomize.

`/base` contains base Grafana configuration
`/example` contains example how to use the manifests.

```
.
├── base
│   ├── grafana.yaml
│   └── kustomization.yaml
├── CODEOWNERS
├── example
│   ├── grafana.yaml
│   ├── kustomization.yaml
│   ├── resources
│   │   ├── dashboards.yaml
│   │   └── datasources.yaml
│   └── secrets
│       ├── grafana-admin-password
│       ├── grafana-git-ssh-key
│       ├── grafana-google-auth-client-secret
│       └── grafana-known_hosts
├── LICENSE
└── README.md

4 directories, 13 files
```

## Example

Check out `kustomization.yaml` in `example/` directory.

You can build example with:

```
kustomize build example/
```

## Requires

- https://github.com/kubernetes-sigs/kustomize

```
go get -u sigs.k8s.io/kustomize
```
