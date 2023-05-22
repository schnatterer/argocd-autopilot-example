argocd-autopilot-example
===

Repo structure created with argocd-autopilot 0.4.12.

```bash
  export GIT_TOKEN=ghp_PcZ...IP0
export GIT_REPO=https://github.com/schnatterer/argocd-autopilot-example

# Basic setup
argocd-autopilot repo bootstrap

# First apparg
argocd-autopilot project create staging
argocd-autopilot app create my-app --app github.com/argoproj-labs/argocd-autopilot/examples/demo-app/ -p staging

# Add stage to app
argocd-autopilot project create production
argocd-autopilot app create my-app --app github.com/argoproj-labs/argocd-autopilot/examples/demo-app/ -p production
``` 

There also is a [branch](https://github.com/schnatterer/autopilot/tree/uninstall) that shows what happens on
```
argocd-autopilot repo uninstall
```

See https://argocd-autopilot.readthedocs.io/en/stable/Getting-Started/
