# RenovateDemoHelm

```
helm repo add ealenn https://ealenn.github.io/charts
helm repo update
helm upgrade -i echo-server ealenn/echo-server --namespace renovate --force
```

Renovate run:
```
docker run \
    --rm \
    -v "./config.js:/usr/src/app/config.js" \
    renovate/renovate \
    --dry-run="true"
```
