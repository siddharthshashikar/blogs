---
layout: post
title: Hardware Forced Security
---
 
Welcome, to a quick introduction & setup session on Intel-SGX SDK for Windows. Before sta
rting the installation, just let me give a brief introduction.

> What is Intel SGX ?
> Why Even bother using Intel SGX ?

So, Intel SGX abbr. Intel Software Gaurd Extension, is a technology that helps application developers, protect selected code & data from discloser and modification. It create something know as enclaves, which are isolated portions of memory, providing a trusted execution enviorment for the applications.

Okay, Okay I get it ?? 

But why do I even bother using something like that?

Hmm, As the saying goes 

“Man is not what he thinks he is, he is what he hides” ― André Malraux.

Every one have secrets, the question is how well you protect it, from not becoming a secret. 

Ok let me give you few basic use-cases or senarios,

>> Health Records.
>> Personal Indentifiable Information (PII).
>> Intellecutal Property.
>> Passwords.
>> Encryption Keys.
>> Bank Data etc.

These are few types of data, that are valuable to companies.   

So, that being said Intel SGX is not the ultimate security requirement for app, but yeah it's definetely place to start.


Now, lets dive deep further into the installation.


![_config.yml]({{ site.baseurl }}/images/config.png)

The easiest way to make your first post is to edit this one. Go into /_posts/ and update the Hello World markdown file. For more instructions head over to the [Jekyll Now repository](https://github.com/barryclark/jekyll-now) on GitHub