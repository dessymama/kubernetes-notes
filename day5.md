☸️ Day 5 – ReplicaSets

📌 Overview

Today, I learned about ReplicaSets, the Kubernetes object responsible for maintaining the desired number of Pods. ReplicaSets automatically replace failed or deleted Pods to ensure applications remain available. I also learned that ReplicaSets are usually managed by Deployments rather than being created directly.


---

📚 What I Learned

A ReplicaSet maintains the desired number of Pods.

If a Pod crashes or is deleted, the ReplicaSet automatically creates a replacement Pod.

ReplicaSets help provide Kubernetes' self-healing capability.

Deployments automatically create and manage ReplicaSets.

DevOps engineers usually create Deployments instead of creating ReplicaSets directly.



---

🧠 Why ReplicaSets?

Applications must remain available even when Pods fail.

ReplicaSets continuously monitor the number of running Pods and ensure the desired number is always maintained.


---

🏗️ Relationship Between Kubernetes Objects

Deployment
      │
      ▼
ReplicaSet
      │
      ▼
Pods

Deployment manages ReplicaSets.

ReplicaSets manage Pods.

Pods run the application containers.



---

🎯 Responsibilities of a ReplicaSet

Maintain the desired number of Pods.

Automatically replace failed Pods.

Create new Pods when existing Pods are deleted.

Remove extra Pods if more than the desired number exist.

Keep applications highly available.



---

💡 Deployment vs ReplicaSet

Deployment	ReplicaSet

Manages ReplicaSets	Manages Pods
Supports rolling updates	Replaces failed Pods
Supports rollbacks	Maintains desired number of Pods
High-level object	Low-level object



---

🚀 DevOps Insight

In production environments, engineers normally create Deployments rather than ReplicaSets. Kubernetes automatically creates and manages ReplicaSets behind the scenes, making application deployment, scaling, and recovery easier.


---

📝 Day 5 Summary

Today, I learned that ReplicaSets ensure the desired number of Pods are always running by automatically replacing failed or deleted Pods. Although ReplicaSets are essential in Kubernetes, they are typically managed by Deployments, allowing DevOps engineers to benefit from rolling updates, rollbacks, and simplified application management.
