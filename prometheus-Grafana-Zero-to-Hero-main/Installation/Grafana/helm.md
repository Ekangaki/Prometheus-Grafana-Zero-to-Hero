# Install using Helm
$ wget https://get.helm.sh/helm-v3.12.0-linux-amd64.tar.gz

$ tar -xvf  helm-v3.12.0-linux-amd64.tar.gz

$ sudo mv linux-amd64  /usr/local/bin

$ helm version

$ sudo snap install helm --classic

## Add helm repo

`helm repo add grafana https://grafana.github.io/helm-charts`

## Update helm repo

`helm repo update`

## Install helm 

`helm install grafana grafana/grafana`

## Expose Grafana Service

`kubectl expose service grafana — type=NodePort — target-port=3000 — name=grafana-ext`
