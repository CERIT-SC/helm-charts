# CERIT-SC Helm Charts

This repository hosts Helm Charts from CERIT-SC

## Adding Helm Repo

```bash
helm repo add cerit-sc https://cerit-sc.github.io/helm-charts
```

## Publishing Helm Charts

To publish a chart from this repository do the following steps:
  - `helm package $CHART_NAME`
  - `git checkout gh-pages`
  - `git add $PACKAGED_CHART`
  - `helm repo index .`
  - `git add index.yaml`
  - `git commit`
  - `git push`
