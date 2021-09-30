A [flash file system](https://en.wikipedia.org/wiki/Flash_file_system) is a file system designed for storing files on flash memory–based storage devices.

Because of the [particular characteristics of flash memory](https://en.wikipedia.org/wiki/Flash_memory_controller), it is best used with either a controller to perform wear leveling and error correction or specifically designed flash file systems, which spread writes over the media and deal with the long erase times of NAND flash blocks. 


https://en.wikipedia.org/wiki/Flash_file_system


The earliest flash file system, managing an array of flash as a freely writable disk, was TrueFFS by M-Systems of Israel, presented as a software product in PC-Card Expo at Santa Clara, California, in July 1992 and patented in 1993.



Around 1994, the PCMCIA, an industry group, approved the Flash Translation Layer (FTL) specification, based on the design of M-Systems' TrueFFS. The specification was authored and jointly proposed by M-Systems and SCM Microsystems, who also provided the first working implementations of FTL.

https://www.sciencedirect.com/topics/computer-science/flash-translation-layer

JFFS was the first flash-specific file system for Linux, but it was quickly superseded by JFFS2, originally developed for NOR flash. Then YAFFS was released in 2002, dealing specifically with NAND flash, and JFFS2 was updated to support NAND flash too.

https://www.embedded.com/flash-101-nand-flash-vs-nor-flash/

UBIFS has been merged since Linux 2.6.22[7] in 2008. UBIFS has been actively developed from its initial merge. UBIFS has documentation hosted at infradead.org along with JFFS2 and MTD drivers. Some initial comparison show UBIFS with compression faster than F2FS.

LogFS, another Linux flash-specific file system, is currently being developed to address the scalability issues of JFFS2.

F2FS (Flash-Friendly File System) was added to the Linux kernel 3.8.[10] Instead of being targeted at speaking directly to raw flash devices, F2FS is designed to be used on flash-based storage devices that already include a flash translation layer, such as SD cards.



Are these flash filesystems used on common SSD drives?

https://www.addictivetips.com/ubuntu-linux-tips/best-ssd-friendly-file-systems-on-linux/

#### TRIM

https://en.wikipedia.org/wiki/Trim_(computing)

#### NVMe


https://wikipedia.org/wiki/NVM_Express
