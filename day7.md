# ☸️ Day 7 – Kubernetes Labels and Selectors

## 📌 Overview

Today, I learned about Kubernetes Labels and Selectors. Labels are key-value pairs attached to Kubernetes objects, while Selectors are used to find and group resources with matching Labels.

## 📚 What I Learned

- Labels identify Kubernetes resources.
- Labels are key-value pairs.
- Selectors find resources based on Labels.
- Services and Deployments use Selectors to locate Pods.
- Labels make resource management easier.

## 🏷️ Example Label

```yaml
labels:
  app: frontend
  env: production
```

## 🎯 Benefits of Labels

- Organize resources
- Group related Pods
- Connect Services to Pods
- Help Deployments manage Pods
- Simplify Kubernetes management

## 💡 Key Lesson

Labels identify resources.

Selectors find resources.

Kubernetes uses both together to manage communication between objects.

## 📝 Day 7 Summary

Today, I learned that Labels are used to identify Kubernetes resources, while Selectors locate resources with matching Labels. Together, they allow Services, Deployments, and other Kubernetes objects to find and manage the correct Pods.
