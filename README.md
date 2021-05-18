# helm-charts
bitbucket-server
bitbucket data center
bitbucket docker image

#Installation
<br>helm repo add bitbucket https://pickybutanidevops.github.io/bitbucket-helm-charts/</br>
<br>helm repo update</br>																					
<br>helm search repo bitbucket</br>																				

<br>helm install bitbucket bitbucket/bitbucket --namespace bitbucket --create-namespace</br>
<br>helm list -n bitbucket</br>

