---
layout: post
title: "Using your development environment, in the cloud as sample my website "
description: ""
category: 
tags: []
---

Since I discovered **c9**: [c9](https://c9.io/), I am using it as my development environment to my blog.

I created my blog using jekyll (https://jekyllrb.com/) with github pages **github pages**: [github pages](https://pages.github.com/), and
my repository is on **thamaraaalves**: [thamaraaalves]((https://github.com/thamaraaalves/thamaraaalves.github.com.)

Create an c9 account. I created with github to transfer my repositories easily. 
![C9 Cloud root]({{ site.baseurl }}assets/posts/c9_root.png "C9 Cloud root")

When I push on c9 instantaneously update on github 
![GitHub master branch]({{ site.baseurl }}assets/posts/github_master_branch.png "GitHub master branch")

Creating post using rake
![Creating post]({{ site.baseurl }}assets/posts/creating_post_rake.png "Creating post")


Additional information - To compress images I use TinyPNG
![Tinypng compress]({{ site.baseurl }}assets/posts/compress_images_tinypng.png "Tinypng compress")
**tinypng**: [tinypng]( https://tinypng.com/)  

Below step by step to run Jekyll on c9.cloud:

Commands:
- gem install jekyll
- jekyll new my-awesome-site
- cd my-awesome-site
- jekyll serve --host $IP --port $PORT --baseurl ''
- 

DOING UPDATES AND POSTING:

**Create a Post**
Create posts easily via rake task:
$ rake post title="Hello World"

The rake task automatically creates a file with properly formatted filename and YAML Front Matter. Make sure to specify your own title. By default, the date is the current date.
The rake task will never overwrite existing posts unless you tell it to.

**Create a Page**
Create pages easily via rake task:
$ rake page name="about.md"
Create a nested page:
$ rake page name="pages/about.md"
Create a page with a "pretty" path:
$ rake page name="pages/about"# this will create the file: ./pages/about/index.html
The rake task automatically creates a page file with properly formatted filename and YAML Front Matter as well as includes the Jekyll Bootstrap "setup" file.

**Publish**
After you've added posts or made changes to your theme or other files, simply commit them to your git repo and push the commits up to GitHub.
$ git add .$ git commit -m "Add new content"$ git push origin master


**Referrences**
**jekyllrb**: [jekyllrb](https://jekyllrb.com/docs/github-pages/)