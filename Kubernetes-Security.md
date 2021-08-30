Kubernetes security is based on the 4C’s of cloud native security: Cloud, Cluster, Container, and Code:


- Cloud (or Corporate Datacenter/Colocation facility): The underlying physical infrastructure is the basis of Kubernetes security. Whether the cluster is built on one’s own datacenter or a cloud provider, basic cloud provider (or physical security) best practices must be observed.
- Cluster: Securing a Kubernetes cluster involves both the configurable components such as the Kubernetes API and security of all the applications that are part of the cluster. Since most cloud-native applications are designed around microservices and APIs, applications are only as secure as the weakest link in the chain of services that comprise the entire application.
- Container: Container design best practices consist of: starting with the smallest code base possible (excluding unnecessary libraries or functions), avoiding granting unnecessary privileges to users in the container, and ensuring that containers are scanned for vulnerabilities at build time.
- Code: Code presents a major attack surface for any Kubernetes environment. Simple policies such as encrypting TCP using TLS handshakes, not exposing unused ports, scanning, and testing regularly can help prevent security issues from arising in a production environment.




https://kubernetes.io/docs/concepts/security/overview/


## Issues

https://www.vmware.com/topics/glossary/content/kubernetes-security

Kubernetes security is important throughout the container lifecycle due to the distributed, dynamic nature of a Kubernetes cluster. Different security approaches are required for each of the three phases of an application lifecycle: build, deploy, and runtime. Kubernetes provides innate security advantages. For example, application containers are typically not patched or updated — instead, container images are replaced entirely with new versions. This enables strict version control and permits rapid rollbacks if a vulnerability is uncovered in new code.

https://techbeacon.com/security/how-track-security-problems-your-kubernetes-deployments


## RBAC

https://cloud.google.com/kubernetes-engine/docs/how-to/role-based-access-control


## Tools

### OPA

https://github.com/open-policy-agent/opa

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


#### Cloud Build

https://security.googleblog.com/2021/05/making-internet-more-secure-one-signed.html

#### Example

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