---
layout: post
title: "Software on rdam and arhus."
description: "software resources"
category: computing
tags: computing 
published: true
comments: false
status: process
---

This page describes some useful Linux tools and statistical programs available on _rdam_ (and on _arhus_ in most instances). These are very short introductions, internet is full of more thorough discussion of each of the topics presented here.

---

# Overview


_rdam_ and _arhus_ have no scheduler and no limits are imposed on the size and the duration of the jobs that users may submit. **With great power comes great responsibility:** you are responsible for ensuring that your jobs do not overload the servers. Below I describe a couple of tools useful for doing that.


 * **screen**: Creates and manages virtual sessions that survive after you logout and can be resumed.
 * **top**: Monitor the server and user processes. 
 

The main statistical packages available on _rdam_ are:
 
 * **R**, **Rstudio**, and **Rstudio server**: Standard installation of *R* and *Rstudio* as well as a browser version of *Rstudio* reachable through a SSH tunnel. 
 * **Matlab R2013b**: Standard installation with VU license.
 * **Ox 7.00**: Installed so that *Ox* runs by default on a single thread.

---

# Linux tools

#### screen 

 1. To create a virtual session named *sname* using screen enter `screen -S sname`. This will result in a blank command prompt, you are in the virtual session. Any job you launch in this session will continue even after you log out. 
 2. To get back to the main session (detach the screen) type `Ctrl-A` and then `d`. 
 1. To reattach a detached session by entering `screen -r sname`. 
 4. To kill the *sname* session enter `exit`. 
 5. To list the existing screen sessions with their status `screen -ls`.
 
 You can find much more detailed (and fancy) tutorials and tips [here](http://www.tecmint.com/screen-command-examples-to-manage-linux-terminals/) and [here](http://www.rackaid.com/blog/linux-screen-tutorial-and-how-to/).
 
#### top 

_top_ is a useful monitoring tool. to access it, simply type `top` at the command line. The first few lines that appear contain server wide statistics.

 * The third line shows the share of total cpu used for:
   1. user processes
   2. system
   3. nice (low priority) processes
   4. idle
 * The fourth line shows the total, used, and available memory. 

Below comes a list of every process, starting with the process id and the user it belongs as well as memory use (RES) and cpu used (%CPU).    

 > Be extremely careful that the memory is not overloaded lest the server grinds to a halt.

_rdam_ has 16 physical cores and can run on up to 32 cores thanks to hyper-threading however performances are optimal when only 16 cores are used. Do not start large jobs when the server is already loaded, you have [other machines]({% post_url 2014-02-28-computing-resources-VU %}) at your disposal.
 
 
 ---
 
# Software
 
#### R, Rstudio, and Rstudio server

_R_ is started by simply typing `R` at the command line. 

[_Rstudio_](https://www.rstudio.com/) provides a graphical user interface for *R* as well as seamless integration with [knitr](http://yihui.name/knitr/) (great tool for reproducible research) and Git (and [Github](https://github.com/), the host of this site) for version control (useful to keep track of code changes and for collaborative work)

_Rstudio Server_ is also installed and _rdam_. It provides an access to _Rstudio_ on _rdam_ in your browser through a SSH tunnel in two steps:

 1. Open a terminal on your machine and enter: `ssh -f -N -L 1234:localhost:8787 VUNetID@rdam`. After you enter your password nothing happens, the SSH tunnel is in the background. How to do this using PuTTY is described [here](http://jimhester.com/post/rstudio-server-through-ssh-tunnel).
 2. Open a browser and point it to `localhost:1234`, enter your VUNetID and password, and here you have _Rstudio_ running on _rdam_.
 
 
#### Matlab

Matlab is installed with the latest stable release R2013b.

 * Start the GUI by typing `matlab` at the command prompt.
 * To execute matlab scripts in the backgroup type `m myfile.m`.

#### Ox 7.00

Ox 7.00 is installed, usage is described on the website of [Charles Bos](http://personal.vu.nl/c.s.bos/resources.html).
 
