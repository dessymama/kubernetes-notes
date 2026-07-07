Day 1 – Introduction to Kubernetes
📌 Overview
Today, I began learning Kubernetes, the industry-standard platform for container orchestration. I learned why Kubernetes was created, how it differs from Docker, and the basic architecture of a Kubernetes cluster.
📚 What I Learned
Kubernetes is an open-source container orchestration platform.
Kubernetes automates deploying, managing, scaling, and recovering containerized applications.
Docker creates and runs containers.
Kubernetes manages containers across one or more servers.
Kubernetes helps keep applications available even when containers or servers fail.
🧠 Why Kubernetes?
Managing a few Docker containers manually is easy.
Managing hundreds or thousands of containers becomes difficult.
Kubernetes solves this by:
Automating deployment
Scaling applications automatically
Restarting failed containers
Managing networking
Performing rolling updates
🐳 Docker vs ☸️ Kubernetes
Docker
Kubernetes
Creates containers
Manages containers
Runs containers
Orchestrates containers
Manual scaling
Automatic scaling
Manual recovery
Self-healing
🏗️ Kubernetes Architecture
Control Plane (Brain)
Responsible for managing the cluster.
Components:
API Server
Scheduler
Controller Manager
etcd
Worker Node
Runs applications.
Components:
Kubelet
Container Runtime
Kube Proxy
📦 Important Kubernetes Terms
Cluster
A group of machines running Kubernetes.
Node
A single machine inside the cluster.
Pod
The smallest deployable unit in Kubernetes.
A Pod usually contains one container.
Deployment
Manages Pods and ensures the desired number of Pods are always running.
Service
Provides stable network access to Pods.
🎯 Key Lesson
Docker is responsible for creating containers.
Kubernetes is responsible for managing containers in production environments.
🚀 DevOps Insight
Most modern cloud applications use Kubernetes because it provides:
High availability
Automatic scaling
Self-healing
Easy deployments
Reliable application management
