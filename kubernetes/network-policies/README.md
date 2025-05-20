# Kubernetes NetworkPolicy Examples

This directory contains Kubernetes NetworkPolicy examples to help you restrict traffic between pods in your Cleura-hosted Kubernetes clusters.

## Examples

- [`deny-all.yaml`](./deny-all.yaml): Denies all ingress and egress traffic for all pods in the namespace.
- [`allow-from-same-namespace.yaml`](./allow-from-same-namespace.yaml): Allows ingress traffic from any other pod in the same namespace.
- [`allow-from-specific-pod.yaml`](./allow-from-specific-pod.yaml): Allows ingress traffic only from pods with a specific label.

## Prerequisites

- A Kubernetes cluster with a CNI plugin that supports NetworkPolicies (e.g., Calico, Cilium).
- `kubectl` configured and connected to the cluster.

## Usage

Apply a policy with:

```bash
kubectl apply -f <file>.yaml
````

For example:

```bash
kubectl apply -f deny-all.yaml
```

To remove all policies in this directory:

```bash
kubectl delete -f .
```

## Learn More

* [Kubernetes NetworkPolicy Documentation](https://kubernetes.io/docs/concepts/services-networking/network-policies/)
* [Cleura Kubernetes Service](https://cleura.com/resources/products-services/containers/)

---

*Made with ❤️ by [Cleura](https://cleura.com)*