---
layout: post
title: "Simple way to create and use Shadow DOM"
description: ""
category: 
tags: [working life, web developer]
---

**Reporting working life**

I've been studying, learning and working as a web developer. Yeahh, at the same time. This experience is amazing, you learn things to put in a real project. 

I met shadow DOM when I was studying web components. Bellow, is a simple code to start creating a simple shadow DOM content. Take a look! Later, I'm gonna explain with details, and better documentation.

    var numberHosts = $('#host').data('numberHosts');
    
    //1. create the shadow dom of the container
    var host = document.querySelectorAll('#host');

    if (host[numberHosts]) {
        var root = host[numberHosts].createShadowRoot();               
        var template = document.querySelectorAll('#template');
        var clone = document.importNode(template[numberHosts].content, true);
    
        kendo.ui.progress($(root.getElementById('Content')) , true);
    
        root.appendChild(clone);
    
        //2. create variables
        var DeleteCalendarButtonID= $(root.getElementById('DeleteButton'));  

    }

Merci! :)