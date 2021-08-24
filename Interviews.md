


## General

http://deliberate-software.com/compassionate-interviewing/

https://review.firstround.com/The-anatomy-of-the-perfect-technical-interview-from-a-former-Amazon-VP

https://builtin.com/software-engineering-perspectives/how-conduct-technical-interview

https://learningforward.org/wp-content/uploads/2020/10/tool-empathy-interviews.pdf

https://triplebyte.com/blog/how-to-interview-engineers


https://www.educative.io/blog/enterprise/tips-conduct-technical-interview

https://github.com/yangshun/tech-interview-handbook

https://github.com/DopplerHQ/awesome-interview-questions




## General Computer Science

https://www.geeksforgeeks.org/most-asked-computer-science-subjects-interview-questions-in-amazon-microsoft-flipkart/amp/

https://www.guru99.com/computer-science-interview-questions.html



## Coding

https://www.educative.io/blog/google-coding-interview-questions

https://www.geeksforgeeks.org/quizzes-on-programming-languages-gq/

https://www.testdome.com/tests

http://eng-web1.eng.famu.fsu.edu/~dommelen/courses/cpp/2_inout/activity/test/index.html

[Interview Coding](Interview-Coding)



## Process vs threads

https://www.tutorialspoint.com/difference-between-process-and-thread

## thread vs coroutines

https://stackoverflow.com/questions/1934715/difference-between-a-coroutine-and-a-thread






## OS questions

https://www.javatpoint.com/operating-system-interview-questions



## Google Cloud Platform

https://www.qfles.com/interview-question/google-cloud-platform-interview-questions

Explain step by step in as much detail as possible what happens when you use Google search from your browser. 

## General Infrastructure

[Interview Infrastructure](Interview-Infrastructure)


## BASICs

Regarding your own computer in  front of you, can you look up information on what hardware components you have? List
CPU, memory, storage, networking details as reported by your operating system (windows, macosx, linux, ...)

How did you look the information up?
What do they say?

Discuss details on each: cpu, memory, storage, network...

How do these things matter when selecting a type of virtual machine in cloud compute services?

## IT and sysadmin questions

https://opensource.com/article/19/7/sysadmin-job-interview-questions

https://www.thebalancecareers.com/information-technology-it-job-interview-questions-2061206

https://www.wgu.edu/blog/common-it-job-interview-questions1911.html







https://www.cosmicnovo.com/2016/12/07/system-administrator-microsoft-interview/






https://www.sanfoundry.com/linux-kernel-interview-questions/

https://www.globalguideline.com/interview_questions/Questions.php?sc=Unix_System_Calls



https://www.globalguideline.com/interview_questions/Questions.php?sc=Signal_Handling


https://narva.webgarden.com/menu/linux-interviw-questions/filesystem-management-1



https://www.howtogeek.com/68563/htg-explains-what-are-the-differences-between-linux-shells/






## Data Science

http://nitin-panwar.github.io/Top-100-Data-science-interview-questions/?utm_campaign=News&utm_medium=Community&utm_source=DataCamp.com


https://towardsdatascience.com/top-30-data-science-interview-questions-7dd9a96d3f5c

https://ds-interviews.org/

https://www.whizlabs.com/blog/top-machine-learning-interview-questions/

[Data Science](Data-Science)

## Data Engineering


[Interview Data Engineering](Interview-Data-Engineering)

## Cloud

https://www.edureka.co/community/cloud-computing/gcp

https://www.gangboard.com/blog/google-cloud-interview-questions-and-answers

https://www.onlineinterviewquestions.com/google-cloud-interview-questions/

https://www.javatpoint.com/cloud-computing-interview-questions



https://www.acte.in/google-cloud-interview-questions-and-answers


https://www.javatpoint.com/cloud-service-models

## Security

[Interview Security](Interview-Security)

## Frontend

https://frontendmasters.com/books/front-end-handbook/2018/practice/interview-q.html

## Backend

https://www.fullstack.cafe/blog/backend-developer-interview-questions

## Networking


[Interview Networking](Interview-Networking)


## Storage

[Interview Storage](Interview-Storage)

## Hardware

https://www.hitequest.com/Hardware/El_hardware.htm

https://mindmajix.com/embedded-hardware-design-development-interview-questions

https://www.slajobs.com/hardware-and-networking-interview-questions/

## General Compute  questions

Describe what is big endian vs little endian

Examples of CPUs that are big endian

How can you tell whether a computer is big endian or not programmatically?

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


## What are processor cores?  

https://quizizz.com/admin/quiz/5ab28f10ba09bf0019b2b33a/cpu-cores

## What is SIMD?
http://ftp.cvut.cz/kernel/people/geoff/cell/ps3-linux-docs/CellProgrammingTutorial/BasicsOfSIMDProgramming.html


## Desktop Support

https://career.guru99.com/top-50-desktop-support-interview-questions/

## Statistics

https://towardsdatascience.com/12-probability-practice-questions-for-data-science-interviews-2ec5230304d9

https://www.digitalvidya.com/blog/bayesian-statistics-interview-questions-answers/

https://intellipaat.com/blog/interview-question/statistics-interview-questions/

https://www.kdnuggets.com/2020/01/data-science-interview-study-guide.html

https://www.analyticsvidhya.com/blog/2021/04/25-probability-and-statistics-questions-to-ace-your-data-science-interviews/

## Math


https://www.testdome.com/d/math-interview-questions/941

https://www.careerride.com/permutations-and-combinations.aspx

https://career.guru99.com/top-20-mathematics-interview-question/

## What is lambda calculus

https://en.wikipedia.org/wiki/Lambda_calculus

## What is Y Combinator



https://en.m.wikipedia.org/wiki/Fixed-point_combinator#Fixed-point_combinators_in_lambda_calculus


## What is Euler's number e?

https://en.m.wikipedia.org/wiki/E_(mathematical_constant)

## DevOps

[Interview DevOps](Interview-DevOps)

https://github.com/bregman-arie/devops-exercises

## Bioinformatics

http://biotech.fyicenter.com/resource/Bioinformatics_Interview_Questions_and_Answers.html

## Reasoning

https://en.wikipedia.org/wiki/Cognitive_reflection_test

https://en.m.wikipedia.org/wiki/Look-and-say_sequence

https://www.firstnaukri.com/career-guidance/65-logical-reasoning-questions-and-answers-for-freshers

https://www.123test.com/logical-reasoning-test/

https://www.lsac.org/lsat/taking-lsat/test-format/logical-reasoning/logical-reasoning-sample-questions

https://www.javatpoint.com/reasoning

## Links




https://github.com/Olshansk/interview

https://www.geeksforgeeks.org/interview-preparation-for-software-developer

https://www.qfles.com/interview-question/

https://www.wisdomjobs.com/e-university/all-skillsets-interview-questions.html

