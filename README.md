# charts

My Helm Chart Repository

## Usage

### Save a package

```bash
helm create mychart
helm package mychart
mv mychart-0.1.0.tgz docs
```

### Update index and upload a package

```bash
helm repo index docs --url https://rurumimic.github.com/charts
git add .
git commit -m "update"
git push origin gh-pages
```

### Install a chart

```bash
helm repo add rurumimic https://rurumimic.github.io/charts
helm repo update
helm search repo rurumimic
helm install my-app rurumimic/<chart-name> --version 0.0.1
```
