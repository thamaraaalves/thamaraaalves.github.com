---
layout: post
title: "Installing polymer in a WebForm project"
description: ""
category: 
tags: [professional, polymer, webcomponents, frontend]
---

After long time I am back. This is my second post since I created this personal site.

This is a professional post. I started to learn polymer, webcomponents, to create a reusable module using webform with c# this month.

Anyway, the question is **"How to install polymer in the project"**?


![2011](/assets/img/posts/webcomponent.png)

First of all, make sure you have nodejs, and git installed in your computer. If not, install them:


**Nodejs**: [Nodejs]( https://nodejs.org/en/)  
**Github**: [Github]( https://desktop.github.com/)  

**Step-by-step:**

1- create a webform/mvc project
2- in node js (with bower, polymer, and git installed)
3- inside the project folder execute the comand: bower init > after set the settings
4- after execute the command: bower install Polymer/polymer --save

**Others comands options:**

comand: bower info polymer
comand: bower info polymer/polymer


If you have some trouble with **git command** in node.js prompt, try this below:

execute the comand: set PATH=%PATH%;C:\Users\Thamara Alves\AppData\Local\Programs\Git\bin

but, change the <Name of the computer>

set PATH=%PATH%;<git path>;
So, like this:
set PATH=%PATH%;C:\Program Files\Git\bin;
Or this: (Notice the (x86) )
set PATH=%PATH%;C:\Program Files (x86)\Git\bin;


**Comands to install new elements:**

inside the path: Scripts\bower_components\webcomponentsjs> 
execute the comand: bower install --save PolymerElements