# charts

My Helm Chart Repository

## Usage

```bash
helm create mychart
helm package mychart
mv mychart-0.1.0.tgz docs
```

```bash
helm repo index docs --url https://rurumimic.github.com/charts
git add .
git commit -m "update"
git push origin gh-pages
```
