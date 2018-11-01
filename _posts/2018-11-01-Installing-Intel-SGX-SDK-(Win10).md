---
layout: post
title: Hardware Forced Security
---

 Welcome, to a quick introduction and setup of Intel-SGX SDK for Windows. Before starting the installation, just let me give a brief introduction.

* What is Intel SGX ?

* Why Even bother using Intel SGX ?

So, Intel SGX abbr. Intel Software Guard Extension, is a technology that helps application developers, protect selected code & data from disclosure and modification. It create something know as enclaves, which are isolated portions of memory, providing a trusted execution environment for the applications.

Okay, I get it ?

But why do I even bother using something like this ?

Hmm, As the saying goes

> “Man is not what he thinks he is, he is what he hides” ― André Malraux.

Everyone have secrets, the question is how well you protect it, from not being a secret.

Okay, let me give you few basic use-cases or scenarios,

* Health Records.

* Personal Identifiable Information (PII).

* Intellectual Property.

* Passwords.

* Encryption Keys.

* Bank Data etc.

These are few types of data, that are extremely valuable into today's data enabled world.  

So, that being said Intel SGX is not __the ultimate security solution__ for applications, but yeah it's definitely a great place to start.

Now, let's dive deep further into the installation. Here I'm assuming that you have already installed some version of Microsoft Visual Studio, if not follow the link [Download Microsoft Visual Studio](https://visualstudio.microsoft.com/downloads/).

But before an application can use Intel SGX, four condition should be met !!!

1. The CPU in the system must support the Intel SGX instructions.

2. The system BIOS must support Intel SGX.

3. Intel SGX must be enabled in the BIOS, and

4. The Intel SGX Platform Software, or PSW, must be installed on that system.

Now, let's get started with Condition 1, in-order to check if your CPU supports Intel SGX instruction kindly visit the [website](https://ark.intel.com/).

Then, click Processors > Intel Core Processors > "Pick your Processor" eg: 7th generation Intel Core i7 Processor > "Select Product Name" > Under Security and Reliability look for "Intel® Software Guard Extensions (Intel® SGX) == YES" .

if __yes__ then great, else [I have your back](https://software.intel.com/en-us/blogs/2016/05/30/usage-of-simulation-mode-in-sgx-enhanced-application).

Now once you are through with Condition 1, let's go to Condition 2 & 3, reboot your PC, open you BIOS Setting check for "Intel Software Guard Extension", just enable it!  

Generally, there are three possible BIOS setting options

1. Enabled

2. Disabled

3. Software Controlled

Not all BIOS manufacturers implement all 3 options and some may even provide no option at all. __Enabled__ setting explicitly enables the Intel SGX, __Disable__ setting explicitly disables the Intel SGX, __Software Controlled__ option allows Intel SGX application to have the BIOS enable it automatically, next time the system reboots.

Ok great, Condition 4 now let's start downloading the SDK and PSW, just follow the links

* [Download Intel SGX SDK for Windows](https://software.intel.com/en-us/sgx-sdk/download).
* [Download Intel SGX PSW for Windows PSW](https://software.intel.com/en-us/sgx-sdk/download).

P.S - Intel asks you fill to a small form, once you have successfully filled the form, it sends you the link to download the SDK & PWS on your registered email address.

Installing Intel SGX SDK is quite easy just follow the GUI installer, but make sure that you have Visual Studio installed and running on your machine.

In the next post we will be discussing "How to build a sample project using the Intel SGX SDK and Visual Studio". Until next time, be better than you were before.

##### References

* [Intel SGX Web Based Training](https://software.intel.com/en-us/documentation/intel-sgx-web-based-training).

* [Intel SGX Webinar](https://software.intel.com/en-us/videos/intel-software-guard-extensions-intel-sgx-webinar).

* [An Introduction to Intel SGX](https://software.intel.com/en-us/videos/an-introduction-to-intel-software-guard-extensions-intel-sgx).