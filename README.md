# Flask Application on Kubernetes

## 📖 Overview
This project demonstrates deploying a Flask application on a Kubernetes cluster using Deployment and Service manifests.

## 🧩 Components
- **Deployment** – runs 2 replicas of the Flask app.
- **Service** – exposes the app on port 30007 (NodePort).

## ⚙️ Run Locally (Minikube)
```bash
# Start minikube
minikube start

# Apply manifests
kubectl apply -f k8s/deployment.yaml
kubectl apply -f k8s/service.yaml

# Get the URL
minikube service flask-service --url
```

## 🧱 Run on GKE

```bash
kubectl apply -f k8s/
kubectl get pods
kubectl get svc
```

## 📬 Output

### Expected response

Hello from Flask on Kubernetes!