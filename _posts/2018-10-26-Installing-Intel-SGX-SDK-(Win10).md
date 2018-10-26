---
layout: post
title: Hardware Forced Security
---
 
Welcome, to a quick introduction and setup of Intel-SGX SDK for Windows. Before starting the installation, just let me give a brief introduction.

* What is Intel SGX ?
* Why Even bother using Intel SGX ?

So, Intel SGX abbr. Intel Software Guard Extension, is a technology that helps application developers, protect selected code & data from disclosure and modification. It create something know as enclaves, which are isolated portions of memory, providing a trusted execution environment for the applications.

Okay, Okay I get it ??

But why do I even bother using something like that ?

Hmm, As the saying goes

> “Man is not what he thinks he is, he is what he hides” ― André Malraux.

Everyone have secrets, the question is how well you protect it, from not being a secret.

Okay, let me give you few basic use-cases or scenarios,

- Health Records.
- Personal Identifiable Information (PII).
- Intellectual Property.
- Passwords.
- Encryption Keys.
- Bank Data etc.

These are few types of data, that are extremely valuable into today's world.  

So, that being said Intel SGX is not the ultimate security rsolution for applications, but yeah it's definitely a great place to start. 

Now, let's dive deep further into the installation.

Here I'm assuming that you have already installed some version of Microsoft Visual Studio, if not follow the link [Download Microsoft Visual Studio](https://visualstudio.microsoft.com/downloads/)

But before an application can use Intel SGX, four condition should be met!!!
1. The CPU in the system must support the Intel SGX instructions.
2. The system BIOS must support Intel SGX.
3. Intel SGX must be enabled in the BIOS, and
4. The Intel SGX Platform Software, or PSW, must be installed on that system.

Now, let's started with Step 1, inorder to check if your CPU supports Intel SGX instruction kindly visit the [website](https://ark.intel.com/)

Then, 
Processors > Intel Core Processors > "Pick your Processor" eg: 7th generation Intel Core i7 Processor > "Select Product Name" > Under Security and Reliability look for "Intel® Software Guard Extensions (Intel® SGX) == YES" 

if __yes__, then great else [ReadMe](https://software.intel.com/en-us/blogs/2016/05/30/usage-of-simulation-mode-in-sgx-enhanced-application).

Now once you are through with step one, let's go to Step 2 & 3, 

// to be added //
 


Ok great, Step 4 for downloading the SDK as well as the PSW kindly follow the links

- [Download Intel SGX SDK for Windows](https://software.intel.com/en-us/sgx-sdk/download)
- [Download Intel SGX PSW for Windows PSW](https://software.intel.com/en-us/sgx-sdk/download)

P.S - Intel asks you fill a small form, once you have successfully filled the form, it sends you the link to download the SDK & PWS on your register email address.


![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub