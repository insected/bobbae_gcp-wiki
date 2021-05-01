# PKI

A public-key infrastructure (PKI) is a set of roles, policies, hardware, software and procedures needed to create, manage, distribute, use, store and revoke digital certificates and manage public-key encryption. The purpose of a PKI is to facilitate the secure electronic transfer of information for a range of network activities such as e-commerce, internet banking and confidential email. It is required for activities where simple passwords are an inadequate authentication method and more rigorous proof is required to confirm the identity of the parties involved in the communication and to validate the information being transferred.

[[https://upload.wikimedia.org/wikipedia/commons/thumb/3/34/Public-Key-Infrastructure.svg/600px-Public-Key-Infrastructure.svg.png]]

https://en.wikipedia.org/wiki/Public_key_infrastructure

# Cloud VPN & IPSec

In [Supported IKE ciphers](https://cloud.google.com/network-connectivity/docs/vpn/concepts/supported-ike-ciphers), you can find details about how Cloud VPN supports multiple [IKE](https://en.wikipedia.org/wiki/Internet_Key_Exchange) ciphers.  IKE is the protocol used to setup a security association (SA) in the [IPSec](https://en.wikipedia.org/wiki/IPsec).  IKE uses [X.509](https://en.wikipedia.org/wiki/X.509) for certificates.  X.509 is a standard defining the format of [public key certificates](https://en.wikipedia.org/wiki/Public-key_cryptography) which are used in TLS/SSL basis for HTTPS.  Base standard for X.509 is [ASN.1](https://en.wikipedia.org/wiki/ASN.1), a kind of IDL for defining data structures that can be serialized and de-serialized.  IKE X.509 certificates
are pre-shared or distributed using DNS or DNSSEC and a [Diffie-Hellman](https://en.wikipedia.org/wiki/Diffie%E2%80%93Hellman_key_exchange) key exchange is used to set up a shared session secret from which cryptographic keys are derived.