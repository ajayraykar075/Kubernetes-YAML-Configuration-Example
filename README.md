📌 Introduction to Kubernetes YAML Configuration 🚀

Kubernetes uses YAML (📝 Yet Another Markup Language) configuration files to define resources such as Pods, Deployments, Services, and ConfigMaps. These YAML files describe the desired state of your Kubernetes resources, which the Kubernetes API server 🖥️ processes and ensures they are created and maintained accordingly.

A basic Kubernetes YAML configuration consists of the following key fields:

    📌 apiVersion: Defines the Kubernetes API version to use.
    📌 kind: Specifies the type of resource (e.g., Pod, Deployment, Service).
    📌 metadata: Provides information about the resource, such as its name and labels.
    📌 spec: Defines the desired state of the resource.

    Basic Deployment Configuration

    apiVersion: apps/v1
kind: Deployment
metadata:
  name: my-app
  labels:
    app: my-app
spec:
  replicas: 3
  selector:
    matchLabels:
      app: my-app
  template:
    metadata:
      labels:
        app: my-app
    spec:
      containers:
        - name: my-app-container
          image: my-app-image:latest
          ports:
            - containerPort: 80



🔍 Breakdown of This Example

✅ Defines a Deployment resource (kind: Deployment) 📦
✅ Uses apps/v1 as the API version 🔄
✅ Metadata assigns the name my-app and label app: my-app 🏷️
✅ Specifies 3 replicas for high availability ⚡
✅ Selects pods with matching labels (matchLabels: app: my-app) 🎯
✅ Defines a Pod template with container details (image, ports, etc.) 🏗️
