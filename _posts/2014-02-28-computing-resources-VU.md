---
layout: post
title: "Computing resources at Econometrics and OR."
description: "computing resources"
category: computing
tags: computing 
published: true
comments: false
status: process
---


# Overview

Here is a brief overview of the machines readily accessible to members of the Econometrics & OR department. Modalities of access and usage of these machines is discussed below.  

Machine | Cores | Memory | Remarks
:------- | -----: | ------: | :-------
_rdam_  | 16 @2.9GHz| 128GB | Detailed user guide below.
_arhus_ |  8 @2.8GHz | 12 GB | Same as above.
_pcoms001_ | 12 @2.3GHz | 128 GB | Administered by the VU.
_pcoms002_ | 12 @2.3GHz | 128 GB | Same as above.
_Lisa_ | 6528 @2.2GHz | 16TB | Administered by Surf Sara. 

---

# pcoms0001 and 002

These machines are administered by the [VU compute service](https://vunet.login.vu.nl/services/pages/detail.aspx?cid=tcm%3a164-330191-16) and accessible from within the VU or through _rdam_ and _arhus_. 

A user manual is provided here [(pdf)](https://vunet.login.vu.nl/_layouts/SharePoint.Tridion.WebParts/redirect.aspx?cid=tcm:164-327430-16). These are essentially similar in software and specs to _rdam_ so also refer to the guide below. *Note that jobs lasting over 24 hours run the risk of being killed without sommations*. 

# Lisa

[Lisa](https://www.surfsara.nl/systems/lisa/description) is a cluster administered by [Surf Sara](https://www.surfsara.nl) (who also provide access to even larger systems) composed of about 500 nodes, each with 8 to 16 cores and 24GB to 32GB of memory. Usage is well [documented here](https://www.surfsara.nl/systems/lisa/usage)

Access to _Lisa_ is subject to a simple and fast [application process](https://www.surfsara.nl/systems/lisa/account) which needs to be supported (by email) by a faculty member with a permanent position. 

---

# Rotterdam and Arhus 

_Rotterdam_, or _rdam_, and _arhus_ are the names of the server financed by the Department of Econometrics & O.R., or NWO, at the VU University
Amsterdam. Members of the department can get an account from <a href="mailto:l.callot@vu.nl">Laurent Callot</a> or <a href="mailto:c.s.bos@vu.nl">Charles
Bos</a> who also maintain these machines.

#### Some definitions

 * _rdam_ and _arhus_ are the machine for which you got an account. 
 * They are known by IP address `145.108.238.26` for rdam and `145.108.238.16` for arhus. They are reachable
from outside the university as well, at these addresses.
 * You received your own login and password. Your login is personal, you
cannot give your password to anybody else.
 *  _rdam_ contains a Tesla card, for GPU computations.
 * Each user has a limited amount of priority, e.g. if two users are working at the machine usually each is limited to 50% of the CPU-time if there is a conflict.
 * For the memory, there is no automatic limit. Please make sure you do not use too much memory, else the machine becomes very slow. 


#### Entering the machine

If this is the first time you login, you will be asked to change your password.

##### Linux, Unix, Apple stuff
To log onto _rdam_ start a terminal and enter `ssh VUnetID@145.108.238.26`, you will be prompted for you password. To exit simply type `exit`.  

##### Windows machine
You can enter the machine using a secure shell program, e.g. [PuTTy](http://www.chiark.greenend.org.uk/%7Esgtatham/putty/). At the VU, send an email to <a href="mailto:ucit-servicedesk@vu.nl">ucit-servicedesk@vu.nl</a> stating that you want access to PuTTY (if you don't have it already). 

Start PuTTY, fill in as host name `145.108.238.26` and save the session under the name _rdam_, then hit the Open button. Fill in your login and password.  When you finish with PuTTY, type `exit`, `ctrl-d`, or just kill the window.

