📌 Introduction to Kubernetes YAML Configuration 🚀

Kubernetes uses YAML (📝 Yet Another Markup Language) configuration files to define resources such as Pods, Deployments, Services, and ConfigMaps. These YAML files describe the desired state of your Kubernetes resources, which the Kubernetes API server 🖥️ processes and ensures they are created and maintained accordingly.

A basic Kubernetes YAML configuration consists of the following key fields:

    📌 apiVersion: Defines the Kubernetes API version to use.
    📌 kind: Specifies the type of resource (e.g., Pod, Deployment, Service).
    📌 metadata: Provides information about the resource, such as its name and labels.
    📌 spec: Defines the desired state of the resource.
