# Keycloak SSO Tutorial on Kubernetes (Grafana Example)

This repo contains all the code needed to follow along with our **[YouTube Tutorial](https://youtu.be/-DQCiaOSlqs)**

## Kubernetes Cluster with Docker Desktop

Set Up Kubernetes Cluster with Docker Desktop: [Kubernetes Cluster Setup](https://kubernetestraining.io/blog/set-up-a-local-kubernetes-cluster-with-docker-desktop)

## Command to Install Keycloak

```
helm repo add bitnami https://charts.bitnami.com/bitnami
helm install keycloak bitnami/keycloak --version 24.4.9 -n keycloak --create-namespace -f keycloak-helm/values.yaml
```

Don't have Helm Installed? See [Install Helm](https://kubernetestraining.io/blog/installing-helm-on-mac-and-windows)

## Command to Install Monitoring Stack

```
helm repo add prometheus https://prometheus-community.github.io/helm-charts/
helm install prometheus prometheus-community/kube-prometheus-stack --version 45.7.1 --namespace monitoring --create-namespace -f monitoring-helm/values.yaml
```

Don't have Helm Installed? See [Install Helm](https://kubernetestraining.io/blog/installing-helm-on-mac-and-windows)

## Testing and Troubleshooting

[Postman](https://www.postman.com/downloads/) is used for testing and troubleshooting

## Decoding JWT Token

[JWT.io](https://jwt.io/) will be used to decode JSON Web Tokens


## Kubernetes Training

If you find these tutorials helpful, check out our [Kubernetes Training course](https://kubernetestraining.io/)
