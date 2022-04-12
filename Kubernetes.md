# Kubernetes: A Containerization Orchestration Tool

## Terminology
Containerization - packaging of an application and its dependencies into essentially a lightweight VM

Cluster - components that represent the control pane, a set of nodes

Nodes - set of machines orchestrated by Kubernetes

Pods - components of the application workload

Pods --> Containers --> Nodes --> Cluster

## Purpose
https://kubernetes.io/docs/concepts/overview/what-is-kubernetes/)

Kubernetes is made to run applications in a distributed fashion to maximize resilience from unexpected events that could otherwise inhibit functionality. 

Kubernetes is commonly used for... 

Service discovery: containers can be exposed using a DNS name or by their own IP address 

Load balancing: can automatically distribute traffic across pods in order to maintain a deployment’s stability 

Storage orchestration: automatically mounts a storage system based on the user’s preferences. For example, local storage, the cloud, etcetera. 

Automated rollouts and rollbacks: like Netflix’s Red-Black strategy, Kubernetes allows you to automatically deploy containers to replace old containers at a controlled rate, and vice versa for rollbacks. 

Automatic bin packing: the user can provide a cluster of nodes to run containerized tasks, and each container is fit onto the nodes in such a way that maximizes resource efficiency in terms of CPU and RAM 

Self-healing: restarts containers that fail, replaces containers, kills containers that don’t respond to health checks, and clients cannot see containers until they are ready for use. 

Secret and configuration management lets you store and manage sensitive information (i.e., passwords, authentication tokens, and SSH keys). Sensitive information can be updated without rebuilding container images and without exposing secrets in your stack configuration. 
## How it Works
A Kubernetes cluster of nodes is created and then a containerized app is deployed on that cluster(s), creating a network of virtual machines. This containerized app is likely to be docker but does not have to be. 

This aforementioned cluster is created via the command line with command line tools, such as Minikube and Kubectl, which let the user interact with it on either a local level or a widespread level. 

## History
Originally a Google project, much of the Kubernetes team came from the Google Borg team which had a similar goal. Launched in 2014 and currently maintained by the Cloud Native Computing Foundation (CNCF) which was formed in 2015 by Google and the Linux foundation. Kubernetes means “helmsman” in Greek and the seven spoked wheel icon comes from both the name and that Kubernetes was known as “Project 7” internally at Google.  

## Strengths and Weaknesses

| Strengths | Weaknesses |
|-----------|------------|
| Runs in the background | Complicated |
| Allows for easy collaboration across teams | Technical issues|
|Can run across many devices | Long waiting times |
|            | Poor User experience |

## Competitors
*Amazon ECS 

*Helios 

*RedHat Open Shift 

*Aptible 

## An Applied Use Case: Mining Stacks

## Our Challenges

## Helpful Links
### Overview
https://kubernetes.io/docs/concepts/overview/
### Tutorials
Basic Kubernetes tutorials: https://kubernetes.io/docs/tutorials/kubernetes-basics/ 

Includes starting a cluster, deploying an app, exploring your app, exposing your app 	publicly, scaling your app, and updating your app. 
### Documentation
Minikube: https://cheatsheet.dennyzhang.com/cheatsheet-minikube-a4 

Kubectl: https://kubernetes.io/docs/reference/kubectl/cheatsheet/ 
### Stacks
Run a Testnet Stacks Node: https://docs.stacks.co/understand-stacks/running-testnet-node 

Mine Testnet Stacks: https://docs.stacks.co/start-mining/testnet 
### Additional
Competitor list: https://www.g2.com/categories/container-orchestration 
