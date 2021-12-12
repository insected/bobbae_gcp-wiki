Google Cloud [encrypts all customer content stored at rest](https://cloud.google.com/security/encryption/default-encryption
), without any action required from the customer, using one or more [encryption mechanisms](Cryptography).

Data for storage is split into chunks, and each chunk is encrypted with a unique data encryption key. These data encryption keys are stored with the data, encrypted with ("wrapped" by) key encryption keys that are exclusively stored and used inside Google's central Key Management Service. [Google's Key Management Service](  https://cloud.google.com/security-key-management  ) is redundant and globally distributed.

All data stored in Google Cloud is encrypted at the storage level using [AES256]( https://wikipedia.org/wiki/Advanced_Encryption_Standard  ), with the exception of a small number of Persistent Disks created before 2015 that use AES128.

Google uses a common cryptographic library, [Tink]( https://github.com/google/tink  ), which incorporates our [FIPS 140-2](https://wikipedia.org/wiki/FIPS_140-2   ) validated module, BoringCrypto, to implement encryption consistently across almost all Google Cloud products. 



https://cloud.google.com/storage/docs/gsutil/addlhelp/SecurityandPrivacyConsiderations#encryption-at-rest
