# k8-rancher

`helm repo add rancher-stable https://releases.rancher.com/server-charts/stable`

`kubectl create namespace cattle-system`

helm install rancher rancher-stable/rancher \
  --namespace cattle-system \
  --set hostname=rancher.home.lab \
  --set replicas=3
  --values values.yaml