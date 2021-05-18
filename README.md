<html>
<meta name="google-site-verification" content="njRQbFZ3zGpqwqbXCXkbZXPxNa0J8pxmPZ3LvFJr-wo" />
  <body>

<br>Bitbucket Helm Chart for Kubernetes</br>

<br>bitbucket-data-center</br>
<br>bitbucket-server</br>
<br>bitbucket-docker-image</br>
<br>AWS EKS</br>
<br>Bitbucket, Postgres, ElasticSearch</br>

#Installation
<br>helm repo add bitbucket https://pickybutanidevops.github.io/bitbucket-helm-charts/</br>
<br>helm repo update</br>																					
<br>helm search repo bitbucket</br>																				

<br>helm install bitbucket bitbucket/bitbucket --namespace bitbucket --create-namespace</br>
<br>helm list -n bitbucket</br>
<br>Get Bitbucket url: helm status bitbucket -n bitbucket</br>
</body>
</html>
