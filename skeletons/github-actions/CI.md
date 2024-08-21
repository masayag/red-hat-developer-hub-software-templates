# GitHub Actions CI Method

## Requirements

The GitHub Actions CI Method will require repository secrets setup before GitHub Actions can run

SECRETS
ArgoCD Secrets

- `OPENSHIFT_SERVER` - The OpenShift server URL that you wish to deploy to using ArgoCD
- `OPENSHIFT_TOKEN` - The token for the OpenShift cluster
- `OPENSHIFT_NAMESPACE` - The namespace you wish to deploy to

CI Variables

- `REGISTRY_NAMESPACE` - The Quay.io registry namespace you wish to push the image to ex. quay.io/<IMAGE_NAMESPACE>/<REGISTRY_URI>:Tag
- `REGISTRY_URI` - The Quay.io image repository, e.g quay.io/<REGISTRY_NAMESPACE>/</REGISTRY_URI>:tag
- `GITOPS_REPO` - The address of the git repository with the argocd manifests
  
CI Secrets

- `REGISTRY_USERNAME` - The Quay.io registry username for the bot
- `REGISTRY_PASSWORD` - The Quay.io registry password for the bot
