# helm-charts
bitbucket-server
bitbucket data center
bitbucket docker image

yum install git
    git clone https://github.com/pickybutanidevops/helm-charts.git && cd helm-charts/

helm lint bitbucket/
helm dependency update bitbucket/

helm repo index bitbucket/


Validate helm template; download/install kubeval
    wget https://github.com/instrumenta/kubeval/releases/latest/download/kubeval-linux-amd64.tar.gz tar xf kubeval-linux-amd64.tar.gz sudo cp kubeval /usr/local/bin

helm template ./bitbucket| kubeval --strict

helm package bitbucket/

helm repo index --url https://pickybutanidevops.github.io/helm-charts/


git add . && git commit -m “Initial commit” && git push origin master

This helm chart is set with AWS ELB - LoadBalancer as a Service(for on premise usage just change service type to ClusterIP and patch with externalIP). 
This Uses AWS - EFS storage, so volume mount for bitbucket data center is mounted with pvc created and check efs is encrypted. 
For on-premise you can use NFS as a storage class. This chart will install Bitbucket-datacenter container, Postgres DB container and elastic search containers.
Please also use external database option when required, refer to Postgres DB container service name when configuring bitbucket.
Note: if you uninstall this helm release chart, pvc created with helm chart installation is not deleted. Retain Policy is set for storage class.


