# Helm Repo
Repository with k8s Helm repo.
Basically it's a repository with helm repo.
Check out this example:
- https://github.com/kmzfs/helm-repo-in-github

## Update Helm Repo
```bash
cd helm
helm package jaeger-all-in-one --destination charts #This will create tgz file with chart in charts directory
helm repo index ./charts #This will create index.yaml file which references jaeger-all-in-one.yaml
git add *
git commit -m "jaeger-all-in-one helm"
git push
```

## Use Helm Repo
```bash
helm repo add jaeger-all-in-one 'https://raw.githubusercontent.com/hansehe/jaeger-all-in-one/master/helm/charts'
helm repo update
helm repo list
```
