[Cryptography](https://wikipedia.org/wiki/Cryptography) is the practice and study of techniques for secure communication in the presence of adversaries.  

A [security protocol](   https://wikipedia.org/wiki/Cryptographic_protocol)  performs a security-related function and applies cryptographic methods, often as sequences of cryptographic primitives. 

There are many [encryption algorithms](https://en.wikipedia.org/wiki/Category:Cryptographic_algorithms).

## Crypto 101
https://www.crypto101.io/

https://cryptobook.nakov.com/

## GCP Encryption

https://cloud.google.com/security/encryption/default-encryption#googles_default_encryption



 


### Google managed certificates

https://cloud.google.com/load-balancing/docs/ssl-certificates/google-managed-certs

### Google Certificate Authority Service

https://cloud.google.com/certificate-authority-service

### Cloud KMS

[Cloud KMS](
Cloud-KMS) is a key management service that lets you manage symmetric and asymmetric cryptographic keys.



## Security Protocols

### TLS

[Transport Layer Security](TLS), and its now-deprecated predecessor, Secure Sockets Layer (SSL), are cryptographic protocols designed to provide communications security over a computer network. 

### PKI

A [public-key infrastructure](PKI) (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke digital certificates and manage public-key encryption. The purpose of a [PKI](https://en.wikipedia.org/wiki/Public_key_infrastructure) is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email.


### HTTPS

[Hypertext Transfer Protocol]( https://wikipedia.org/wiki/HTTPS   ) Secure (HTTPS) is an extension of the Hypertext Transfer Protocol (HTTP). In HTTPS, the communication protocol is encrypted using Transport Layer Security (TLS) or, formerly, Secure Sockets Layer (SSL). The protocol is therefore also referred to as HTTP over TLS, or HTTP over SSL.

### SSH

The [Secure Shell Protocol](https://phoenixnap.com/kb/ssh-to-connect-to-remote-server-linux-or-windows) (SSH) is a cryptographic network protocol for operating network services securely over an unsecured network. 


[OpenSSH](https://en.wikipedia.org/wiki/OpenSSH) can be used as a kind of VPN in addition to normal login, tunneling use cases.

### cert manager 

[cert-manager](https://cert-manager.io/docs/) is a native Kubernetes certificate management controller. It can help with issuing certificates from a variety of sources, such as [Let’s Encrypt]( https://letsencrypt.org/  
) , [HashiCorp Vault](  https://www.vaultproject.io/  ), [Venafi]( https://www.venafi.com/ ), a simple signing key pair, or self signed.



It is loosely based upon the work of [kube-lego]( https://github.com/jetstack/kube-lego   ) and has borrowed some wisdom from other similar projects such as kube-cert-manager.

### Let's Encrypt

To enable HTTPS on your website, you need to get a certificate (a type of file) from a Certificate Authority (CA). [Let’s Encrypt](  https://letsencrypt.org/ ) is a CA. 

### ACME

[Automatic certificate management environment]( https://tools.ietf.org/html/rfc8555  ).


#### acme.sh

https://github.com/acmesh-official/acme.sh



### IPSec

[Internet Protocol Security](https://www.cloudflare.com/learning/network-layer/what-is-ipsec/) (IPsec) is a secure network protocol suite that authenticates and encrypts the packets of data to provide secure encrypted communication between two computers over an Internet Protocol network. 


#### Complexity of IPSec

https://www.schneier.com/academic/archives/2003/12/a_cryptographic_eval.html


### IKE

[Internet Key Exchange](https://en.wikipedia.org/wiki/Internet_Key_Exchange) is the protocol used to set up a security association (SA) in the IPsec protocol suite. IKE builds upon the Oakley protocol and [ISAKMP](  https://wikipedia.org/wiki/Internet_Security_Association_and_Key_Management_Protocol ). IKE uses [X.509](  https://en.m.wikipedia.org/wiki/X.509  ) certificates for authentication ‒ either pre-shared or distributed using DNS (preferably with DNSSEC) ‒ and a Diffie–Hellman key exchange to set up a shared session secret from which cryptographic keys are derived. 

Cloud VPN supports  [some IKE ciphers](https://cloud.google.com/network-connectivity/docs/vpn/concepts/supported-ike-ciphers).


### X.509

[X.509](  https://wikipedia.org/wiki/X.509  ) is a standard defining the format of [public key certificates](https://en.wikipedia.org/wiki/Public-key_cryptography) which are used in TLS/SSL basis for HTTPS.  Base standard for X.509 is [ASN.1](https://en.wikipedia.org/wiki/ASN.1), a kind of [IDL](  https://en.m.wikipedia.org/wiki/Interface_description_language ) for defining data structures that can be serialized and de-serialized.  

### Diffie-Hellman 

[Diffie–Hellman key exchange](https://en.wikipedia.org/wiki/Diffie%E2%80%93Hellman_key_exchange) is a method of securely exchanging cryptographic keys over a public channel and was one of the first public-key protocols as conceived by Ralph Merkle and named after Whitfield Diffie and Martin Hellman. DH is one of the earliest practical examples of public key exchange implemented within the field of cryptography. Published in 1976 by Diffie and Hellman, this is the earliest publicly known work that proposed the idea of a private key and a corresponding public key.


Traditionally, secure encrypted communication between two parties required that they first exchange keys by some secure physical means, such as paper key lists transported by a trusted courier. The Diffie–Hellman key exchange method allows two parties that have no prior knowledge of each other to jointly establish a shared secret key over an insecure channel. This key can then be used to encrypt subsequent communications using a [symmetric-key cipher](  https://brilliant.org/wiki/symmetric-ciphers/ ).

### SSL and TLS
https://dev.to/techschoolguru/a-complete-overview-of-ssl-tls-and-its-cryptographic-system-36pd



### SSL Certificates
https://www.digitalocean.com/community/tutorials/openssl-essentials-working-with-ssl-certificates-private-keys-and-csrs

### Creating Self-Signed Certificates and Keys with OpenSSL
https://mariadb.com/docs/security/data-in-transit-encryption/create-self-signed-certificates-keys-openssl/

### PEM, DER, CRT, and CER: X.509 Encodings and Conversions
https://www.ssl.com/guide/pem-der-crt-and-cer-x-509-encodings-and-conversions/


### From HTTP to HTTPS
https://www.prakharsrivastav.com/posts/from-http-to-https-using-go/

### HTTP Client and Server using Go
https://youngkin.github.io/post/gohttpsclientserver/

### Create Your Own SSL Certificate Authority for Local HTTPS Development
https://deliciousbrains.com/ssl-certificate-authority-for-local-https-development/

### Cryptographic hash

A [cryptographic hash]( https://wikipedia.org/wiki/Cryptographic_hash_function  ) function (CHF) is a mathematical algorithm that maps data of arbitrary size (often called the "message") to a bit array of a fixed size (the "hash value", "hash", or "message digest"). It is a one-way function, that is, a function which is practically infeasible to invert.

https://qvault.io/cryptography/how-sha-2-works-step-by-step-sha-256/


### ECC Encryption / Decryption
https://cryptobook.nakov.com/asymmetric-key-ciphers/ecc-encryption-decryption

### Creating Elliptic Curve Keys using OpenSSL
https://www.scottbrady91.com/openssl/creating-elliptical-curve-keys-using-openssl

### OpenSSL Elliptic Curve Operations
https://wiki.openssl.org/index.php/Command_Line_Elliptic_Curve_Operations

### Smallstep
https://smallstep.com/

### Monocypher
https://monocypher.org/

### Git object model

http://shafiul.github.io/gitbook/1_the_git_object_model.html

### Vulnerability in Cryptography libraries

https://kerkour.com/blog/rust-cryptography-ecosystem/

### Post Quantum Cryptography 

https://nakedsecurity.sophos.com/2022/04/11/openssh-goes-post-quantum-switches-to-qubit-busting-crypto-by-default/

### Cypher agility

https://paragonie.com/blog/2019/10/against-agility-in-cryptography-protocols

### Cryptography Tutorial

https://toc.cryptobook.us/