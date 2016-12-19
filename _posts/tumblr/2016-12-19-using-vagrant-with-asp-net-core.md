---
layout: post
title: "Using vagrant with Asp .Net Core"
description: ""
category: 
tags: [vagrant, webdevelopment, deployment]
---

Basically install vagrant 
[Vagrant](https://www.vagrantup.com/downloads.html), but what's vagrant?  
Vagrant allow you to create and configure lightweight, reproducible, and portable development environments.

To make vagrant works you need a virtual machine, I  usually use Virtual Box 
 [VirtualBox](https://www.virtualbox.org/wiki/Downloads)

**Create an ASP.NET core project in Visual Studio**
![Asp net core project]({{ site.baseurl }}assets/posts/create_project.png "Asp net core project")


**Or just clone or download my project from gitlab**
**Gitlab project**: [Gitlab project]( https://gitlab.com/thamaraaalves/aspcorevagrant/)  


... download the vagrant file [vagrant file]({{ site.url }}/assets/Vagrantfile.file) directly.

After you install vagrant, and virtualbox, create an asp core project, insert the vagrant file you've downloaded on the project root,
open the prompt, and run the commands:
- vagrant plugin install vagrant-hostmanager
**You should see something like this:**
![Asp net core project]({{ site.baseurl }}assets/posts/vagrant_host_manager.png "Asp net core project")

- vagrant up
**You should see something like this:**
![Asp net core project]({{ site.baseurl }}assets/posts/vagrant_up.png "Asp net core project")

Vagrant up will install the windows server 2012, and build up everything, will take time, be patience, wait, and enjoy. 

Merci * -- * 


