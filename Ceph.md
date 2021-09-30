[Ceph](https://ceph.io/en/) implements object, block and file storage.

https://ceph.io/en/discover/technology/

#### Ceph Object storage

The Ceph RGW object storage service provides  S3 API compatibility with a robust set of security, tiering, and interoperability features. 


https://docs.ceph.com/en/latest/architecture/#ceph-object-storage


#### Ceph Block storage

Ceph RBD (RADOS Block Device) block storage stripes virtual disks over objects within a Ceph storage cluster, distributing data and workload across all available devices for extreme scalability and performance. RBD disk images are [thinly provisioned](https://searchstorage.techtarget.com/definition/thin-provisioning), support both read-only snapshots and writable clones, and can be asynchronously mirrored to remote Ceph clusters in other data centers for disaster recovery or backup, making Ceph RBD the leading choice for block storage in public/private cloud and virtualization environments.

https://docs.ceph.com/en/latest/architecture/#ceph-block-device

#### Ceph File Storage



The Ceph File System (CephFS) is a robust, fully-featured POSIX-compliant distributed filesystem as a service with snapshots, quotas, and multi-cluster mirroring capabilities. CephFS files are striped across objects stored by Ceph for extreme scale and performance. Linux systems can mount CephFS filesystems natively, via a FUSE-based client, or via an NFSv4 gateway.


https://docs.ceph.com/en/latest/architecture/#ceph-file-system




