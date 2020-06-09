# TOC

## Video

You can see the talk registration [here](https://youtu.be/jhkYvEgNT4A).

## Slides
- [`slides`](./slides): the talk slides about Authentication, Access control, Confidentiality and Audit in Kubernetes

## Demo
- [`demo`](./demo)
  - [`infra`](./demo/infra): the infrastrucure code to deploy the cluster nodes and the network
  - [`kubeadm`](./demo/kubeadm): the Kubernetes API server configuration for audit via Kubeadm
  - [`falcosecurity/evolution`](https://github.com/falcosecurity/evolution/tree/82ccd2e3216a57e633dda46407cb566f552d0a92/deploy/kubernetes/kernel-and-k8s-audit): the resources used to deploy Falco the non-official way on-top-of Kubernetes
  - [`falcosecurity/event-generator`](https://github.com/falcosecurity/event-generator/tree/4870f6d146e878cab8dc4c041089d0f1dfe13a0a/deployment): the resources used to demonstrate the tracing features of Falco

