# Kubernetes Minikube Sample App

## Objective
Deploy and manage an NGINX app in a local Kubernetes cluster using Minikube.

---

## Files
- `deployment.yaml`: Defines the deployment for the app.
- `service.yaml`: Exposes the app using a NodePort.
- `output/`: Screenshots of each step.

---

## Commands Used

```bash
minikube start
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl get pods
kubectl get services
kubectl scale deployment hello-world-deployment --replicas=4
kubectl describe pod <pod-name>
kubectl logs <pod-name>
