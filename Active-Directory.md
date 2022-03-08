[Google Managed Service for Microsoft Active Directory](https://cloud.google.com/managed-microsoft-ad) (AD) is a highly available, hardened Google Cloud service running actual [Microsoft AD](https://en.wikipedia.org/wiki/Active_Directory) that enables you to manage authentication and authorization for your AD-dependent workloads, automate AD server maintenance and security configuration, and connect your on-premises AD domain to the cloud.

https://cloud.google.com/managed-microsoft-ad

Active Directory (AD) is a directory service developed by Microsoft for Windows domain networks. It is included in most Windows Server operating systems as a set of processes and services.


https://cloud.google.com/blog/products/identity-security/managed-service-for-microsoft-active-directory-is-ga

Managed Microsoft AD runs actual Microsoft Active Directory domain controllers on Windows virtual machines to ensure application compatibility. The service creates and maintains the domain controllers for you, reducing the maintenance tasks you need to manage.

https://engineering.sada.com/using-gcp-managed-active-directory-to-simplify-domain-authentication-4d8b4a12985b

## Domain Services

Active Directory Domain Services (AD DS) is the foundation stone of every Windows domain network. 

https://docs.microsoft.com/en-us/windows-server/identity/ad-ds/get-started/virtual-dc/active-directory-domain-services-overview

## Directory Services

Active Directory Lightweight Directory Services (AD LDS), formerly known as Active Directory Application Mode (ADAM), is an implementation of LDAP protocol for AD DS.

https://docs.microsoft.com/en-us/previous-versions/windows/desktop/adam/what-is-active-directory-lightweight-directory-services

### LDAP

The Lightweight Directory Access Protocol (LDAP) is an open, vendor-neutral, industry standard application protocol for accessing and maintaining distributed directory information services over an Internet Protocol (IP) network.

https://en.wikipedia.org/wiki/Lightweight_Directory_Access_Protocol

## Certificate Services

Active Directory Certificate Services (AD CS) establishes an on-premises [public key infrastructure](PKI). 


https://www.securew2.com/blog/active-directory-certificate-services-ad-cs-explained

## Federation Services

Active Directory Federation Services (AD FS) is a single sign-on service. 

https://docs.microsoft.com/en-us/windows-server/identity/active-directory-federation-services

## Rights Management

Active Directory Rights Management Services (AD RMS, known as Rights Management Services or RMS before Windows Server 2008) is a server software for information rights management shipped with Windows Server. 


https://docs.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2012-r2-and-2012/hh831364(v=ws.11)

## SIDs


Security Identifier (commonly abbreviated SID) is a unique, immutable identifier of a user, user group, or other security principal. A security principal has a single SID for life (in a given domain), and all properties of the principal, including its name, are associated with the SID.

https://en.wikipedia.org/wiki/Security_Identifier

## Federating  Active Directory with GCP Cloud Identity with GCDS

https://cloud.google.com/architecture/identity/federating-gcp-with-active-directory-synchronizing-user-accounts