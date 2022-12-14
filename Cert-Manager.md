

[Cert-manager](https://cert-manager.io/docs/) is a native [Kubernetes](Kubernetes) certificate management controller. It can help with issuing certificates from a variety of sources, such as [Let’s Encrypt](https://letsencrypt.org/), HashiCorp [Vault](https://www.vaultproject.io/), [Venafi](https://www.venafi.com/), a simple signing key pair, or self signed.



## Certificate Manager

https://cloud.google.com/certificate-manager/docs

Certificate Manager lets you acquire and manage TLS (SSL) certificates for use with Cloud Load Balancing. 



## Google managed certificates

Google-managed SSL certificates are Domain Validation (DV) certificates that Google Cloud obtains and manages for your domains. They support multiple hostnames in each certificate, and Google renews the certificates automatically.

https://cloud.google.com/load-balancing/docs/ssl-certificates/google-managed-certs


## LetsEncrypt

To enable HTTPS on your website, you need to get a certificate (a type of file) from a Certificate Authority (CA). [Let’s Encrypt](https://letsencrypt.org/
) is a free and automated CA. In order to get a certificate for your website’s domain from Let’s Encrypt, you have to demonstrate control over the domain. With Let’s Encrypt, you do this using software that uses the [ACME protocol](https://datatracker.ietf.org/doc/html/rfc8555)  which typically runs on your web host.



## Auto provision of Kubernetes certs

A Tutorial on installing and securing ingress to your Kubernetes cluster using NGINX.

https://cert-manager.io/docs/tutorials/acme/ingress/

## Examples

An example to automatically provision and manage TLS certificates in GKE.

https://gregdaybreak.medium.com/auto-provisioning-lets-encrypt-wildcard-certificates-with-cert-manager-on-gke-8665994b9ae8

### kube-lego

Deprecated method to automatically request certificates for kubernetes ingress resources from Let's Encrypt.

https://github.com/jetstack/kube-lego

### GKE Ingress with Let's Encrypt using Cert-Manager

https://kosyfrances.com/ingress-gce-letsencrypt/

### Securing NGINX Ingress

https://cert-manager.io/docs/tutorials/acme/ingress/