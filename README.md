# helmfile-example
example using helmfile, helm, sops, werf, kind

```
kind create cluster
export WERF_HELM3_MODE=1
. envs/default/envs.sh
helmfile --helm-binary=werf --interactive --file=helmfile.yaml apply
```
