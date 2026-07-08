☸️ Day 3 – Understanding Deployments
📌 Overview
Today, I learned about Deployments, one of the most important Kubernetes objects. Deployments manage Pods by ensuring the correct number of Pods are running and automatically replacing failed Pods.
📚 What I Learned
A Deployment manages one or more Pods.
Deployments automatically create Pods.
If a Pod fails, the Deployment creates a replacement.
Deployments make application updates easier.
They support scaling and rolling updates.
🧠 Why Do We Need Deployments?
Creating a Pod directly is not ideal because:
If the Pod crashes, it stays down.
There is no automatic recovery.
Updating applications is difficult.
A Deployment solves these problems by continuously monitoring Pods.
🏗️ How Deployments Work
Deployment
     │
     ▼
 ReplicaSet
     │
     ▼
    Pods
The Deployment tells Kubernetes how many Pods should exist and keeps that desired state.
🎯 Main Responsibilities of a Deployment
Create Pods
Replace failed Pods
Scale applications up or down
Perform rolling updates
Roll back to previous versions if needed
📈 Scaling Example
Suppose you want 3 Pods running.
If one Pod crashes:
Desired Pods: 3

Running:
Pod 1 ✅
Pod 2 ❌
Pod 3 ✅
Kubernetes automatically creates:
Pod 4 ✅
so there are 3 running Pods again.
🔄 Rolling Updates
Instead of stopping the whole application, Kubernetes updates Pods one at a time.
Benefits:
No downtime
Safer deployments
Easy rollback if something goes wrong
💡 Key Lesson
A Deployment ensures that the desired number of Pods are always running and automatically recovers from Pod failures.
