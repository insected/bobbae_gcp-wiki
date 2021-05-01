Cryptography is the practice and study of techniques for secure communication in the presence of third parties called adversaries. More generally, cryptography is about constructing and analyzing protocols that prevent third parties or the public from reading private messages; various aspects in information security such as data confidentiality, data integrity, authentication, and non-repudiation are central to modern cryptography. Modern cryptography exists at the intersection of the disciplines of mathematics, computer science, electrical engineering, communication science, and physics. 

A security protocol (cryptographic protocol or encryption protocol) is an abstract or concrete protocol that performs a security-related function and applies cryptographic methods, often as sequences of cryptographic primitives. A protocol describes how the algorithms should be used. A sufficiently detailed protocol includes details about data structures and representations, at which point it can be used to implement multiple, interoperable versions of a program.

https://en.m.wikipedia.org/wiki/Cryptography

# PKI

A public-key infrastructure (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke digital certificates and manage public-key encryption. The purpose of a PKI is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email. It is required for activities where simple passwords are an inadequate authentication method and more rigorous proof is required to confirm the identity of the parties involved in the communication and to validate the information being transferred.

[[https://upload.wikimedia.org/wikipedia/commons/thumb/3/34/Public-Key-Infrastructure.svg/600px-Public-Key-Infrastructure.svg.png]]



# SSH

The Secure Shell Protocol (SSH) is a cryptographic network protocol for operating network services securely over an unsecured network.[1] Typical applications include remote command-line, login, and remote command execution, but any network service can be secured with SSH.

[[https://upload.wikimedia.org/wikipedia/commons/thumb/0/0f/Ssh_binary_packet_alt.svg/500px-Ssh_binary_packet_alt.svg.png]]



# TLS

Transport Layer Security (TLS), and its now-deprecated predecessor, Secure Sockets Layer (SSL), are cryptographic protocols designed to provide communications security over a computer network. Several versions of the protocols are widely used in applications such as email, instant messaging, and voice over IP, but its use as the Security layer in HTTPS remains the most publicly visible.


# HTTPS

Hypertext Transfer Protocol Secure (HTTPS) is an extension of the Hypertext Transfer Protocol (HTTP). It is used for secure communication over a computer network, and is widely used on the Internet. In HTTPS, the communication protocol is encrypted using Transport Layer Security (TLS) or, formerly, Secure Sockets Layer (SSL). The protocol is therefore also referred to as HTTP over TLS, or HTTP over SSL.

# cert manager 

cert-manager is a native Kubernetes certificate management controller. It can help with issuing certificates from a variety of sources, such as Let’s Encrypt, HashiCorp Vault, Venafi, a simple signing key pair, or self signed.

It will ensure certificates are valid and up to date, and attempt to renew certificates at a configured time before expiry.

It is loosely based upon the work of kube-lego and has borrowed some wisdom from other similar projects such as kube-cert-manager.

# letsEncrypt 

To enable HTTPS on your website, you need to get a certificate (a type of file) from a Certificate Authority (CA). Let’s Encrypt is a CA. In order to get a certificate for your website’s domain from Let’s Encrypt, you have to demonstrate control over the domain. With Let’s Encrypt, you do this using software that uses the ACME protocol which typically runs on your web host.

# ACME

Automatic certificate management environment.

https://tools.ietf.org/html/rfc8555



# Cloud VPN & IPSec

Internet Protocol Security (IPsec) is a secure network protocol suite that authenticates and encrypts the packets of data to provide secure encrypted communication between two computers over an Internet Protocol network. It is used in virtual private network.




## IKE

In [Supported IKE ciphers](https://cloud.google.com/network-connectivity/docs/vpn/concepts/supported-ike-ciphers), you can find details about how Cloud VPN supports multiple [IKE](https://en.wikipedia.org/wiki/Internet_Key_Exchange) ciphers. 

IKE is the protocol used to setup a security association (SA) in the [IPSec](https://en.wikipedia.org/wiki/IPsec).  IKE uses [X.509](https://en.wikipedia.org/wiki/X.509) for certificates.  

## X.509

X.509 is a standard defining the format of [public key certificates](https://en.wikipedia.org/wiki/Public-key_cryptography) which are used in TLS/SSL basis for HTTPS.  Base standard for X.509 is [ASN.1](https://en.wikipedia.org/wiki/ASN.1), a kind of IDL for defining data structures that can be serialized and de-serialized.  

## Diffie-Hellman 

IKE X.509 certificates
are pre-shared or distributed using DNS or DNSSEC and a [Diffie-Hellman](https://en.wikipedia.org/wiki/Diffie%E2%80%93Hellman_key_exchange) key exchange is used to set up a shared session secret from which cryptographic keys are derived.
