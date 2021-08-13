[Cryptography](https://en.m.wikipedia.org/wiki/Cryptography) is the practice and study of techniques for secure communication in the presence of third parties called adversaries. More generally, cryptography is about constructing and analyzing protocols that prevent third parties or the public from reading private messages; various aspects in information security such as data confidentiality, data integrity, authentication, and non-repudiation are central to modern cryptography. Modern cryptography exists at the intersection of the disciplines of mathematics, computer science, electrical engineering, communication science, and physics. 

A security protocol (cryptographic protocol or encryption protocol) is an abstract or concrete protocol that performs a security-related function and applies cryptographic methods, often as sequences of cryptographic primitives. A protocol describes how the algorithms should be used. A sufficiently detailed protocol includes details about data structures and representations, at which point it can be used to implement multiple, interoperable versions of a program.

There are many [encryption algorithms](https://en.wikipedia.org/wiki/Category:Cryptographic_algorithms).

## PKI

A [public-key infrastructure](https://en.wikipedia.org/wiki/Public_key_infrastructure) (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke digital certificates and manage public-key encryption. The purpose of a [PKI](https://en.wikipedia.org/wiki/Public_key_infrastructure) is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email. It is required for activities where simple passwords are an inadequate authentication method and more rigorous proof is required to confirm the identity of the parties involved in the communication and to validate the information being transferred.




## SSH

The [Secure Shell Protocol](https://phoenixnap.com/kb/ssh-to-connect-to-remote-server-linux-or-windows) (SSH) is a cryptographic network protocol for operating network services securely over an unsecured network. Typical applications include remote command-line, login, and remote command execution, but any network service can be secured with SSH.


[OpenSSH](https://en.wikipedia.org/wiki/OpenSSH) can be used as a kind of VPN in addition to normal login, tunneling use cases.

## TLS

[Transport Layer Security](https://www.csoonline.com/article/3246212/what-is-ssl-tls-and-how-this-encryption-protocol-works.html) (TLS), and its now-deprecated predecessor, Secure Sockets Layer (SSL), are cryptographic protocols designed to provide communications security over a computer network. Several versions of the protocols are widely used in applications such as email, instant messaging, and voice over IP, but its use as the Security layer in HTTPS remains the most publicly visible.


## HTTPS

[Hypertext Transfer Protocol]( https://en.m.wikipedia.org/wiki/HTTPS   ) Secure (HTTPS) is an extension of the Hypertext Transfer Protocol (HTTP). It is used for secure communication over a computer network, and is widely used on the Internet. In HTTPS, the communication protocol is encrypted using Transport Layer Security (TLS) or, formerly, Secure Sockets Layer (SSL). The protocol is therefore also referred to as HTTP over TLS, or HTTP over SSL.

## cert manager 

[cert-manager](https://cert-manager.io/docs/) is a native Kubernetes certificate management controller. It can help with issuing certificates from a variety of sources, such as [Let’s Encrypt]( https://letsencrypt.org/  
) , [HashiCorp Vault](  https://www.vaultproject.io/  ), [Venafi]( https://www.venafi.com/ ), a simple signing key pair, or self signed.

It will ensure certificates are valid and up to date, and attempt to renew certificates at a configured time before expiry.

It is loosely based upon the work of [kube-lego]( https://github.com/jetstack/kube-lego   ) and has borrowed some wisdom from other similar projects such as kube-cert-manager.

## Let's Encrypt

To enable HTTPS on your website, you need to get a certificate (a type of file) from a Certificate Authority (CA). [Let’s Encrypt](  https://letsencrypt.org/ ) is a CA. In order to get a certificate for your website’s domain from Let’s Encrypt, you have to demonstrate control over the domain. With Let’s Encrypt, you do this using software that uses the ACME protocol which typically runs on your web host.

## ACME

[Automatic certificate management environment]( https://tools.ietf.org/html/rfc8555  ).


See also: https://github.com/acmesh-official/acme.sh


## IPSec

[Internet Protocol Security](https://www.cloudflare.com/learning/network-layer/what-is-ipsec/) (IPsec) is a secure network protocol suite that authenticates and encrypts the packets of data to provide secure encrypted communication between two computers over an Internet Protocol network. It is used in virtual private network.

See also: https://www.schneier.com/academic/archives/2003/12/a_cryptographic_eval.html


## IKE

[Internet Key Exchange](https://en.wikipedia.org/wiki/Internet_Key_Exchange) is the protocol used to set up a security association (SA) in the IPsec protocol suite. IKE builds upon the Oakley protocol and [ISAKMP](  https://en.m.wikipedia.org/wiki/Internet_Security_Association_and_Key_Management_Protocol ). IKE uses [X.509](  https://en.m.wikipedia.org/wiki/X.509  ) certificates for authentication ‒ either pre-shared or distributed using DNS (preferably with DNSSEC) ‒ and a Diffie–Hellman key exchange to set up a shared session secret from which cryptographic keys are derived. In addition, a security policy for every peer which will connect must be manually maintained.

Cloud VPN supports  [some IKE ciphers](https://cloud.google.com/network-connectivity/docs/vpn/concepts/supported-ike-ciphers).


## X.509

[X.509](  https://en.m.wikipedia.org/wiki/X.509  ) is a standard defining the format of [public key certificates](https://en.wikipedia.org/wiki/Public-key_cryptography) which are used in TLS/SSL basis for HTTPS.  Base standard for X.509 is [ASN.1](https://en.wikipedia.org/wiki/ASN.1), a kind of IDL for defining data structures that can be serialized and de-serialized.  

## Diffie-Hellman 

[Diffie–Hellman key exchange](https://www.math.ucla.edu/~baker/40/handouts/rev_DH/node1.html) is a method of securely exchanging cryptographic keys over a public channel and was one of the first public-key protocols as conceived by Ralph Merkle and named after Whitfield Diffie and Martin Hellman. DH is one of the earliest practical examples of public key exchange implemented within the field of cryptography. Published in 1976 by Diffie and Hellman, this is the earliest publicly known work that proposed the idea of a private key and a corresponding public key.


Traditionally, secure encrypted communication between two parties required that they first exchange keys by some secure physical means, such as paper key lists transported by a trusted courier. The Diffie–Hellman key exchange method allows two parties that have no prior knowledge of each other to jointly establish a shared secret key over an insecure channel. This key can then be used to encrypt subsequent communications using a [symmetric-key cipher](  https://brilliant.org/wiki/symmetric-ciphers/ ).



## Cryptographic hash

A [cryptographic hash]( https://en.m.wikipedia.org/wiki/Cryptographic_hash_function  ) function (CHF) is a mathematical algorithm that maps data of arbitrary size (often called the "message") to a bit array of a fixed size (the "hash value", "hash", or "message digest"). It is a one-way function, that is, a function which is practically infeasible to invert.

https://qvault.io/cryptography/how-sha-2-works-step-by-step-sha-256/

### Git object model

http://shafiul.github.io/gitbook/1_the_git_object_model.html
