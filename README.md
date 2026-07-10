# Vault Infrastructure

Manejo do HashiCorp Vault no cluster Kubernetes.

## Estrutura

```
vault-infra/
├── namespace.yaml
├── serviceaccount.yaml
├── clusterrolebinding.yaml
├── configmap.yaml
├── deployment.yaml
└── service.yaml
```

## Deploy

```bash
kubectl apply -f .
```

## Acesso

```bash
kubectl port-forward -n vault svc/vault 8200:8200
```

Acesse o UI: http://localhost:8200/ui
