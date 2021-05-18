# helm-charts
<br><b>bitbucket-data-center</b></br>
<br>bitbucket-server</br>
<br>bitbucket-docker-image</br>
<br>AWS EKS</br>
<br>bitbucket, Postgres, ElasticSearch</br>

#Installation
<br>helm repo add bitbucket https://pickybutanidevops.github.io/bitbucket-helm-charts/</br>
<br>helm repo update</br>																					
<br>helm search repo bitbucket</br>																				

<br>helm install bitbucket bitbucket/bitbucket --namespace bitbucket --create-namespace</br>
<br>helm list -n bitbucket</br>
<br>Get Bitbucket url: helm status bitbucket -n bitbucket</br>

