# helm-charts
bitbucket-server
bitbucket data center
bitbucket docker image

#Installation
helm repo add bitbucket https://pickybutanidevops.github.io/bitbucket-helm-charts/
helm repo update
helm search repo bitbucket

helm install bitbucket bitbucket/bitbucket --namespace bitbucket --create-namespace
helm list -n bitbucket

