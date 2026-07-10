# ☸️ Day 6 – Kubernetes Namespaces

## 📌 Overview

Today, I learned about Kubernetes Namespaces, which are used to organize and separate resources inside a Kubernetes cluster. Namespaces allow multiple teams and applications to share the same cluster while keeping resources logically separated.

## 📚 What I Learned

- A Namespace divides a Kubernetes cluster into separate environments.
- Namespaces help organize Kubernetes resources.
- Different teams can work independently within the same cluster.
- Resources in different Namespaces can have the same name.
- Namespaces are commonly used in production environments.

## 🎯 Benefits of Namespaces

- Organization of resources
- Logical isolation between teams and environments
- Access control using RBAC
- Resource management using limits

## 🏗️ Common Namespace Examples

- Development
- Testing
- Production

## 📦 Default Kubernetes Namespaces

- default – Used when no Namespace is specified.
- kube-system – Contains Kubernetes system components.
- kube-public – Contains publicly accessible resources.
- kube-node-lease – Stores node heartbeat information.

## 💡 Key Lesson

Namespaces provide logical separation inside a Kubernetes cluster. They do not create separate clusters.

## 🚀 DevOps Insight

Production Kubernetes environments commonly use Namespaces to separate development, staging, and production workloads while sharing the same cluster infrastructure.

## 📝 Day 6 Summary

Today, I learned that Kubernetes Namespaces help organize, isolate, and manage resources within a cluster. They are important for multi-team environments and production Kubernetes management.
