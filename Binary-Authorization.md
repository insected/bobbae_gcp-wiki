[Binary Authorization](https://cloud.google.com/binary-authorization/docs) is a service on Google Cloud that provides software supply-chain security for applications that run in the cloud. 

[https://www.youtube.com/watch?v=mi50OJq6wd0](https://www.youtube.com/watch?v=mi50OJq6wd0)


### Container image binary authorization


[Binary Authorization](https://cloud.google.com/binary-authorization/) is a deploy-time security control that ensures only trusted container images are deployed on Google Kubernetes Engine or [Cloud Run](Cloud-run). With Binary Authorization, you can require images to be signed by trusted authorities during the development process and then enforce signature validation when deploying. By enforcing validation, you can gain tighter control over your container environment by ensuring only verified images are integrated into the build-and-release process.





### Binary Authorization Attestations with Voucher

An [attestor](https://cloud.google.com/binary-authorization/docs/creating-attestations-voucher) is a Google Cloud resource that Binary Authorization uses to verify the attestation at container image deploy time. Attestors contain the public key that corresponds to the private key used by a signer to sign the container image digest and create the attestation. 

The Binary Authorization enforcer uses the attestor at deploy time to limit which container images are allowed to be deployed to those with an accompanying, verifiable attestation created prior to deployment.


### Binary Authorization for Borg

https://cloud.google.com/security/binary-authorization-for-borg

## DevSecOps

Whether you call it [DevOps](DevOps) or [DevSecOps](DevSecOps), it has always been ideal to include security as an integral part of the entire app life cycle. 