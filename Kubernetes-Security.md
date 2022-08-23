Kubernetes security is based on the [4C’s of cloud native security](Kubernetes provides innate security advantages. For example, application containers are typically not patched or updated — instead, container images are replaced entirely with new versions. This enables strict version control and permits rapid rollbacks if a vulnerability is uncovered in new code.).




https://kubernetes.io/docs/concepts/security/overview/


## Issues

https://www.vmware.com/topics/glossary/content/kubernetes-security

Kubernetes security is important throughout the container lifecycle due to the distributed, dynamic nature of a Kubernetes cluster. Different security approaches are required for each of the three phases of an application lifecycle: build, deploy, and runtime. 

https://techbeacon.com/security/how-track-security-problems-your-kubernetes-deployments

## Using Google-managed SSL certificates 

https://www.infracloud.io/blogs/secure-containers-cosign-distroless-images


## RBAC

https://cloud.google.com/kubernetes-engine/docs/how-to/role-based-access-control

## Workload identity for GKE
https://medium.com/@jonatanweckl/how-to-implement-workload-identity-on-google-kubernetes-engine-clusters-f86b414976dc

https://cloud.google.com/kubernetes-engine/docs/concepts/workload-identity

## Tools

### OPA

https://www.openpolicyagent.org/


https://github.com/open-policy-agent/opa

### Kubernetes cluster outage due to misconfigured OPA Gatekeeper 
https://dev.to/fourstepper/dealing-with-a-google-kubernetes-engine-cluster-outage-2kf1

### TerraScan

https://github.com/accurics/terrascan

### Falco

https://github.com/falcosecurity/falco

### Kube Linter

https://github.com/stackrox/kube-linter



### SigStore

https://www.sigstore.dev/

### Distroless

"Distroless" images contain only your application and its runtime dependencies. They do not contain package managers, shells or any other programs you would expect to find in a standard Linux distribution.

https://github.com/GoogleContainerTools/distroless

### CoSign

Container Signing, Verification and Storage in an [OCI](https://opencontainers.org/) registry.


https://github.com/sigstore/cosign


###  Cloud Build CoSign

https://security.googleblog.com/2021/05/making-internet-more-secure-one-signed.html

### CoSign and distroless images

https://www.infracloud.io/blogs/secure-containers-cosign-distroless-images

### Clair

https://github.com/quay/clair

### Checkov

https://github.com/bridgecrewio/checkov


### Admission Controllers

https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/

#### Validating Webhooks

https://kmitevski.com/writing-a-kubernetes-validating-webhook-using-python/


### StackRox

https://www.stackrox.io/blog/kubernetes-security-101/



[StackRox](https://www.stackrox.com/post/2020/11/stackrox-integrates-with-google-artifact-registry/) provides full life cycle security across build, deploy, and runtime phases for your Google Kubernetes Engine (GKE), Google Compute Engine (GCE), or Anthos environments. 

StackRox can be used to enforce security policies for [GKE](GKE) with [Cloud Run](Cloud-Run). 





### Encrypt Secrets at rest

https://kubernetes.io/docs/tasks/administer-cluster/securing-a-cluster/#encrypt-secrets-at-rest


### Aqua 

https://www.aquasec.com/products/kubernetes-security/


### Kubescape

https://github.com/armosec/kubescape

### Kube bench

https://github.com/aquasecurity/kube-bench

### Kube hunter

https://github.com/aquasecurity/kube-hunter

### Kube audit

https://github.com/Shopify/kubeaudit

### NeuVector

https://neuvector.com/

### Audit2RBAC

https://github.com/liggitt/audit2rbac

### Illuminatio

https://github.com/inovex/illuminatio

### Prisma

https://www.paloaltonetworks.com/prisma/cloud/cloud-workload-protection-platform/container-security

### KubeSec

https://kubesec.io/