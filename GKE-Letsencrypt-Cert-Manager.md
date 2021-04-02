# cert manager

cert-manager is a native Kubernetes certificate management controller. It can help with issuing certificates from a variety of sources, such as Let’s Encrypt, HashiCorp Vault, Venafi, a simple signing key pair, or self signed.


https://cert-manager.io/docs/




## Google managed certificates

Google-managed SSL certificates are Domain Validation (DV) certificates that Google Cloud obtains and manages for your domains. They support multiple hostnames in each certificate, and Google renews the certificates automatically.

https://cloud.google.com/load-balancing/docs/ssl-certificates/google-managed-certs


## letsEncrypt

To enable HTTPS on your website, you need to get a certificate (a type of file) from a Certificate Authority (CA). Let’s Encrypt is a CA. In order to get a certificate for your website’s domain from Let’s Encrypt, you have to demonstrate control over the domain. With Let’s Encrypt, you do this using software that uses the ACME protocol which typically runs on your web host.


https://letsencrypt.org/

## auto provision of Kubernetes certs



https://gregdaybreak.medium.com/auto-provisioning-lets-encrypt-wildcard-certificates-with-cert-manager-on-gke-8665994b9ae8