☸️ Day 2 – Understanding Pods
📌 Overview
Today, I learned about Pods, the smallest deployable unit in Kubernetes. I understood why Kubernetes uses Pods instead of managing containers directly and how Pods are used to run applications.
📚 What I Learned
A Pod is the smallest unit Kubernetes creates and manages.
A Pod usually contains one container.
Multiple containers can exist in one Pod if they work closely together.
Containers inside the same Pod share:
Network
Storage
IP address
📦 What is a Pod?
A Pod is a wrapper around one or more containers.
Instead of Kubernetes creating containers directly, it creates Pods, and the Pods contain the containers.
🧠 Why Pods?
Pods provide:
Shared networking
Shared storage
Easier communication between related containers
Better application management
🏗️ Pod Structure
Kubernetes Cluster
        │
        ▼
      Worker Node
        │
        ▼
        Pod
        │
        ▼
   Docker Container
🧩 Single-Container Pod
This is the most common type.
Pod
 └── Nginx Container
🧩 Multi-Container Pod
Sometimes two containers work together.
Example:
Pod
 ├── Web Application
 └── Log Collector
Both share the same network and storage.
🎯 Benefits of Pods
Easy application deployment
Shared resources
Efficient communication
Simplified management
Supports microservices architecture
💡 Key Lesson
Kubernetes does not manage containers directly.
It manages Pods, and Pods contain the containers.
