---
layout: post
title: "Simple way to create and use Shadow DOM"
description: ""
category: 
tags: [working life, web developer]
---

**Reporting working life**

I've been studying, learning and working as a web developer. Yeahh, at the same time. This experience is amazing, you learn things to put in a real project. 

I met shadow DOM when I was studying web components. Bellow, is a simple code to start creating a simple shadow DOM content (in this case ready document could be call more than once). 
Take a look! 
Later, I'm gonna explain with details, and with better documentation.

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
        var DeleteButtonID= $(root.getElementById('DeleteButton'));  
        
     if ($('#host').data('numberHosts')==0 || $('#host').data('numberHosts')>0) 
        $('#host').data('numberHosts', $('#host').data('numberHosts')+1);
    }

One important thing is when you create a shadow DOM, your ROOT will be encapsulate, to customize, for example if you are using KENDO UI framework, 
you have to important the stylesheet, putting the code bellow inside the tags <style> </style>:


    /* to use external style sheets inside shadow dom */
    @import url('<%= Page.ResolveUrl("~/Content/kendo/kendo.common.min.css") %>')
     
    
** References and fonts: **   
[W3 Shadow DOM](https://www.w3.org/TR/shadow-dom/)
[HTML5 Rocks](http://www.html5rocks.com/en/tutorials/webcomponents/shadowdom/)

Merci! :)