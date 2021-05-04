# helm-charts
Atlassian
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
