📌 Overview
Today, I learned about Kubernetes Services, which provide a stable way to access Pods. Since Pods can be created, destroyed, and recreated at any time, their IP addresses can change. A Service gives applications a permanent endpoint for communication.
📚 What I Learned
A Service exposes Pods to users or other applications.
Services provide a stable IP address and DNS name.
Even if Pods are replaced, the Service continues working.
Services distribute traffic across multiple Pods (load balancing).
🤔 Why Do We Need Services?
Imagine you have a Deployment with 3 Pods.
Pod A → IP: 10.0.0.2
Pod B → IP: 10.0.0.3
Pod C → IP: 10.0.0.4
If Pod A crashes, Kubernetes creates a new Pod:
Pod D → IP: 10.0.0.8
The Pod IP changed.
Without a Service, users would have to know the new IP every time a Pod changes.
A Service solves this by providing one permanent address.
🌐 Types of Kubernetes Services
1. ClusterIP (Default)
Used for communication inside the cluster only.
Not accessible from the internet.
2. NodePort
Exposes the application through a port on every Node.
Can be accessed from outside the cluster.
3. LoadBalancer
Creates a cloud load balancer (AWS, Azure, GCP).
Best for production internet-facing applications.
4. ExternalName
Maps a Service to an external DNS name.
🎯 Responsibilities of a Service
Give Pods a stable network identity.
Load balance traffic between Pods.
Allow applications to communicate reliably.
Hide changing Pod IP addresses.
💡 Key Lesson
Pods are temporary.
Services are permanent.
Applications connect to Services, not directly to Pods.


DevOps Insight
In production:
Users connect to a Service.
The Service forwards traffic to healthy Pods.
If a Pod fails, Kubernetes creates a new one, and the Service automatically sends traffic to it.
This provides high availability without users noticing failures.
📝 Day 4 Summary
Today, I learned that Kubernetes Services provide a stable way to access Pods. Services solve the problem of changing Pod IP addresses by giving applications a permanent endpoint and distributing traffic across healthy Pods.
