# ostad-moudule-6-k8s

## Overview
This repository contains all Kubernetes manifests for deploying a full-stack Node.js application with MongoDB and Mongo Express.

## Files
- `namespace.yaml`: Namespace definition (`ostad-student-system`)
- `ostad-server-deployment.yaml`: Deployment for the server API
- `ostad-server-service.yaml`: Service for the server API
- `ostad-ui-deployment.yaml`: Deployment for the frontend UI
- `ostad-ui-service.yaml`: Service for the frontend UI
- `mongo-configmap.yaml`: ConfigMap for MongoDB initialization
- `mongo-deployment.yaml`: Deployment for MongoDB
- `mongo-service.yaml`: ClusterIP Service for MongoDB
- `mongo-secret.yaml`: Secret for MongoDB credentials
- `mongo-express-deployment.yaml`: Deployment for Mongo Express UI
- `mongo-express-service.yaml`: NodePort Service for Mongo Express
- `ingress.yaml`: Ingress resource for routing `ostad.local` and `mongo.local`

## Usage
```bash
kubectl apply -R -f ./k8s
Author
Adib Azfer