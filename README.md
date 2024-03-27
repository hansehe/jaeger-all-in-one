# Jaeger Tracing - All In One

[![Artifact HUB](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/jaeger-all-in-one)](https://artifacthub.io/packages/search?repo=jaeger-all-in-one)

The Jaeger tracing all-in-one service enables jaeger for development purposes, check out:
- https://www.jaegertracing.io/docs/1.55/getting-started/

## Run With Docker
```bash
docker-compose -f docker-compose.yml up
```

Access jaeger at: 
- http://localhost:16686/

Access hotrod tracing demo at: 
- http://localhost:8080/

## Use Helm Repo
```bash
helm repo add jaeger-all-in-one https://raw.githubusercontent.com/hansehe/jaeger-all-in-one/master/helm/charts
helm repo update
```
```bash
helm install jaeger-all-in-one jaeger-all-in-one/jaeger-all-in-one
```

