- [do you have and cloud certification ?   what kinds?](#do-you-have-and-cloud-certification-----what-kinds-)
- [do you wish to study and pass certification tests?](#do-you-wish-to-study-and-pass-certification-tests-)
- [have you applied and tested for certificates?  success or failures?](#have-you-applied-and-tested-for-certificates---success-or-failures-)
- [virtualization](#virtualization)
- [Hypervisors](#hypervisors)
- [aws, azure, gcp](#aws--azure--gcp)
- [docker](#docker)
- [kubernetes](#kubernetes)
- [General Compute  questions](#general-compute--questions)
  * [Describe what is big endian vs little endian](#describe-what-is-big-endian-vs-little-endian)
  * [Examples of CPUs that are big endian](#examples-of-cpus-that-are-big-endian)
  * [How can you tell whether a computer is big endian or not programmatically?](#how-can-you-tell-whether-a-computer-is-big-endian-or-not-programmatically-)
  * [Why does the endianness matter?](#why-does-the-endianness-matter-)
- [why do modern computers use two's compliment representation](#why-do-modern-computers-use-two-s-compliment-representation)
- [what is "Turing complete"](#what-is--turing-complete-)
- [what is "Von Neumann" architecture](#what-is--von-neumann--architecture)
- [RISC vs CISC](#risc-vs-cisc)
- [example of RISC](#example-of-risc)
  * [Classic RISC  pipeline](#classic-risc--pipeline)
- [Process vs threads](#process-vs-threads)
- [thread vs coroutines](#thread-vs-coroutines)
- [What are processor cores?](#what-are-processor-cores-)
- [What is SIMD?](#what-is-simd-)
- [OS questions](#os-questions)
- [Linux](#linux)
- [Linux, Unix](#linux--unix)
- [RAM, cache, cache-line, registers, hard disk, flash disk, different parts of computer](#ram--cache--cache-line--registers--hard-disk--flash-disk--different-parts-of-computer)

<small><i><a href='http://ecotrust-canada.github.io/markdown-toc/'>Table of contents generated with markdown-toc</a></i></small>





## do you have and cloud certification ?   what kinds?

Discuss details

## do you wish to study and pass certification tests?

What kind of certificates are you interested in?
Why?

## have you applied and tested for certificates?  success or failures?
```
AWS, Azure, GCP?

How did you prepare?

Cloud academy?
Cloud guru?
Linux Academy?
Coursera?
Udemy?
etc.?
```





## virtualization

https://www.unixarena.com/2019/08/virtualization-hypervisor-basic-interview-questions.html/

https://www.javatpoint.com/virtualization-in-cloud-computing

## Hypervisors

Types of hypervisors.

https://vapour-apps.com/what-is-hypervisor/

## aws, azure, gcp

https://www.javatpoint.com/aws-vs-azure-vs-google-cloud-platform

## docker

https://www.edureka.co/blog/interview-questions/docker-interview-questions/

## kubernetes

https://www.edureka.co/blog/interview-questions/kubernetes-interview-questions/

## General Compute  questions

### Describe what is big endian vs little endian

### Examples of CPUs that are big endian

### How can you tell whether a computer is big endian or not programmatically?

```
#include <stdio.h> 

/* function to show bytes in memory, from location start to start+n*/
void show_mem_rep(char *start, int n) 
{ 
	int i; 
	for (i = 0; i < n; i++) 
		printf(" %.2x", start[i]); 
	printf("\n"); 
} 

/*Main function to call above function for 0x01234567*/
int main() 
{ 
int i = 0x01234567; 
show_mem_rep((char *)&i, sizeof(i)); 
//getchar(); 
return 0; 
} 
```

If this prints `67 45 23 01` then little endian.  If you get `01 23 45 67` then big endian.

### Why does the endianness matter?
What happens when you write a binary file on big endian machine and
read it back in little endian machine?

what happens when you write non-binary data, e.g. ASCII, or UTF-8 data, into the files and read them back on different endian machines, does it matter much?

What needs to be done for binary data in the IP header read from network?

## why do modern computers use two's compliment representation

https://en.wikipedia.org/wiki/Two%27s_complement

https://stackoverflow.com/questions/1125304/why-prefer-twos-complement-over-sign-and-magnitude-for-signed-numbers

## what is "Turing complete"

https://en.wikipedia.org/wiki/Turing_completeness


## what is "Von Neumann" architecture

https://www.thecrazyprogrammer.com/2019/02/difference-between-von-neumann-and-harvard-architecture.html

## RISC vs CISC
https://www.microcontrollertips.com/risc-vs-cisc-architectures-one-better/

## example of RISC

https://binaryterms.com/risc-processor.html

### Classic RISC  pipeline

Why?

https://en.wikipedia.org/wiki/Classic_RISC_pipeline

## Process vs threads

https://www.tutorialspoint.com/difference-between-process-and-thread

## thread vs coroutines

https://stackoverflow.com/questions/1934715/difference-between-a-coroutine-and-a-thread

## What are processor cores?  

https://quizizz.com/admin/quiz/5ab28f10ba09bf0019b2b33a/cpu-cores

## What is SIMD?
http://ftp.cvut.cz/kernel/people/geoff/cell/ps3-linux-docs/CellProgrammingTutorial/BasicsOfSIMDProgramming.html



## OS questions

https://www.javatpoint.com/operating-system-interview-questions


## Linux

https://www.javatpoint.com/linux-interview-questions

## Linux, Unix

https://www.educba.com/linux-system-administration-interview-questions/

https://www.educba.com/linux-system-administration-interview-questions/

https://www.softwaretestinghelp.com/unix-vs-linux/



https://www.whizlabs.com/blog/top-linux-interview-questions-answers/

https://www.globalguideline.com/interview_questions/Questions.php?sc=Linux_OS_Management



https://www.guru99.com/unix-interview-questions.html

## RAM, cache, cache-line, registers, hard disk, flash disk, different parts of computer

https://medium.com/software-design/why-software-developers-should-care-about-cpu-caches-8da04355bb8a
