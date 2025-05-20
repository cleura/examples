# Kubernetes Examples for Cleura Cloud

This directory contains practical Kubernetes examples tailored for Cleura-hosted Kubernetes clusters. Whether you're just getting started or managing production-grade workloads, these manifests can help streamline your operations.

## 📂 Available Examples
- [`network-policies`](./network-policies): Secure pod-to-pod traffic with Kubernetes NetworkPolicies.

## 🚀 How to Use

Make sure `kubectl` is configured to point to your Cleura cluster.

Apply an example:

```bash
kubectl apply -f <example>/
```

Check the resources:

```bash
kubectl get all
```

Clean up:

```bash
kubectl delete -f <example>/
```

## 🧰 Prerequisites

- A Cleura Kubernetes cluster
- `kubectl` installed and authenticated
- CNI plugin that supports NetworkPolicies (for relevant examples)

## 📖 Resources

- [Cleura Kubernetes Documentation](https://cleura.com/resources/products-services/containers/)
- [Kubernetes Official Docs](https://kubernetes.io/docs/)

---

*Made with ❤️ by [Cleura](https://cleura.com)*
