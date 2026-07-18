# ☸️ Day 11 – Creating Your First Pod

## 📌 Overview

Today, I learned how to create my first Kubernetes Pod using a YAML Manifest. Kubernetes reads the YAML file and creates the Pod automatically.

## 📚 What I Learned

- Pods can be created using YAML files.
- kubectl apply -f creates Kubernetes resources.
- kubectl get pods displays running Pods.
- kubectl describe pod provides detailed Pod information.
- kubectl delete pod removes a Pod.

## 📄 Sample Commands

- kubectl apply -f pod.yaml
- kubectl get pods
- kubectl describe pod nginx-pod
- kubectl delete pod nginx-pod

## 💡 Key Lesson

Using YAML files makes Kubernetes deployments repeatable, consistent, and easy to manage with Git.

## 🚀 DevOps Insight

DevOps engineers use YAML files together with kubectl to deploy and manage Kubernetes resources in production.

## 📝 Day 11 Summary

Today, I learned how to create, inspect, and delete a Kubernetes Pod using YAML and kubectl. This is a fundamental Kubernetes skill and an important part of Infrastructure as Code.
