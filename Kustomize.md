

[Kustomize](https://kustomize.io/) introduces a template-free way to customize application configuration that simplifies the use of off-the-shelf applications. Now, built into kubectl as apply -k.


Kustomize provides a solution for customizing Kubernetes resource configuration free from templates and DSLs.

Kustomize lets you customize raw, template-free YAML files for multiple purposes, leaving the original YAML untouched and usable as is.

Kustomize targets kubernetes; it understands and can patch kubernetes style API objects. It’s like make, in that what it does is declared in a file, and it’s like sed, in that it emits edited text.

https://kubectl.docs.kubernetes.io/guides/introduction/kustomize/

## Extending

Kustomize offers a plugin framework allowing people to write their own resource generators and transformers.

Write a plugin when changing generator options or transformer configs doesn’t meet your needs.

- A generator plugin could be a helm chart inflator, or a plugin that emits all the components (deployment, service, scaler, ingress, etc.) needed by someone’s 12-factor application, based on a smaller number of free variables.

- A transformer plugin might perform special container command line edits, or any other transformation beyond those provided by the builtin (namePrefix, commonLabels, etc.) transformers.

https://kubectl.docs.kubernetes.io/guides/extending_kustomize/


## Comparison to Helm.



https://harness.io/blog/helm-vs-kustomize/