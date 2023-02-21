argocd-autopilot-example
===

Repostructure create with argocd-autopilot 0.4.12.

```
  export GIT_TOKEN=ghp_PcZ...IP0
export GIT_REPO=https://github.com/schnatterer/autopilot

argocd-autopilot repo bootstrap
argocd-autopilot project create testing
argocd-autopilot app create hello-world --app github.com/argoproj-labs/argocd-autopilot/examples/demo-app/ -p testing --wait-timeout 2m
``` 

There also is a [branch](https://github.com/schnatterer/autopilot/tree/uninstall) that shows what happens on
```
argocd-autopilot repo uninstall
```

See https://argocd-autopilot.readthedocs.io/en/stable/Getting-Started/
