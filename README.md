# Keycloak SSO Tutorial on Kubernetes (Grafana Example)

This repo contains all the code needed to follow along with our **[YouTube Tutorial](https://link-here)**

## Command to Install Keycloak

```
helm install keycloak bitnami/keycloak --version 24.4.9 -n keycloak --create-namespace -f keycloak-helm/values.yaml
```

## Command to Install Monitoring Stack

```
helm install prometheus prometheus-community/kube-prometheus-stack --version 45.7.1 --namespace monitoring --create-namespace
```

## Testing and Troubleshooting

[Postman](https://www.postman.com/downloads/) is used for testing and troubleshooting

## Decoding JWT Token

[JWT.io](https://jwt.io/) will be used to decode JSON Web Tokens


## Kubernetes Training

If you find these tutorials helpful, check out our [Kubernetes Training course](https://kubernetestraining.io/)
