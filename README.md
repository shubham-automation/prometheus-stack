# prometheus-stack

helm repo add prometheus-community https://prometheus-community.github.io/helm-charts

helm repo update

helm upgrade --install kube-prometheus-stack prometheus-community/kube-prometheus-stack -f values.yaml

kubectl apply -f prometheus_rules.yaml
