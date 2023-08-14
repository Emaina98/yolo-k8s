# Kubernetes Configuration Files

This directory contains the Kubernetes configuration files for deploying and managing the services in your application. Each YAML file corresponds to a specific Kubernetes resource.

## Table of Contents

- [Services](#services)
- [Deployments](#deployments)
- [ConfigMaps and Secrets](#configmaps-and-secrets)
- [Persistent Volumes and Claims](#persistent-volumes-and-claims)

## Services

- [frontend-service.yaml](k8s/frontend-service.yaml): Exposes the frontend application to the internet using a LoadBalancer type service.
- [backend-service.yaml](k8s/backend-service.yaml): Exposes the backend application within the cluster using a ClusterIP type service.

## Deployments

- [frontend-deployment.yaml](k8s/frontend-deployment.yaml): Deploys and manages the frontend application pods.
- [backend-deployment.yaml](k8s/backend-deployment.yaml): Deploys and manages the backend application pods.

## ConfigMaps and Secrets

- [app-configmap.yaml](k8s/app-configmap.yaml): Defines configuration data as a ConfigMap for the applications.
- [db-secret.yaml](k8s/db-secret.yaml): Defines sensitive data (e.g., database credentials) as a Secret.

## Ingress

- [app-ingress.yaml](k8s/app-ingress.yaml): Defines Ingress rules for routing external traffic to the services.

## Persistent Volumes and Claims

- [mongo-pv.yaml](k8s/mongo-pv.yaml): Defines a PersistentVolume (PV) for MongoDB storage.
- [mongo-pvc.yaml](k8s/mongo-pvc.yaml): Defines a PersistentVolumeClaim (PVC) to bind to the PV for MongoDB.

## Usage

To deploy the resources to your Kubernetes cluster, use the following commands:

```bash
kubectl apply -f k8s/
To launch the application click on this ip:
[yolo k8s link](http://34.135.226.223/)
