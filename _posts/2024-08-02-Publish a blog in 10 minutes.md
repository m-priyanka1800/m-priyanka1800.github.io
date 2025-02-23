---
title: Publish a blog in 10 minutes
description: Setup and publish a blog directly from your browser in under 10 mintues!
date: 2024-08-02 12:22:00 +0530
categories: [Website,Blog]
tags: [github_pages,jekyll]     # TAG names should always be lowercase
image:
  path: ../assets/img/Setup_blog.png
  alt: Setup a blog in minutes using GitHub Pages
---

# Setting up a blog


When it comes to setting up a blog there are plenty of GUI-friendly drag and drop options out there like Blogger, Medium and Wix. And while these websites are a great option to get started, many of them force you to forgo copywrite ownership on your content and have full control on how your work can be distributed and monetized.

Today we will go over a great alternative to these sites that allows retain full ownership of your content: GitHub Pages. We will go through how to setup and deploy a site in under 10 mintues. You can follow along, to create a site that looks just like this one. And all you need is a web browser.

> You don't have to restrict yourself to just creating a blog, this type of website can also be used to share your portfolio to client/ potential employers. Do keep in mind all the information on the site is publically available, so avoid sharing any sensitive information.
{: .prompt-tip }

## GitHub Pages

This is a GitHub service which allows you to host a website directly from a GitHub repository. If that sounds too complicated don't worry, all this means is that you can deploy a publicly available static website from code on your account.

## How-To

1. Log into [`Github.com`](https://github.com/) and create an account using an email address and pick a username.
2. To create the website we will be using a Jekyll theme called [`Chirpy`](https://github.com/cotes2020/jekyll-theme-chirpy). It is clean, interactive and renders well on mobile-devices. To reuse this theme click on this link: <i class="fa fa-arrow-right" aria-hidden="true"></i> [`chirpy-starter`](https://github.com/cotes2020/chirpy-starter) code repo.
3. Create a copy of this code for your own repository by clicking on `Use this template` > `Create a new repository`
4. Under repository name write a name in this format: **<<github_user_name>>.github.io**. Where `github_user_name` refers the your GitHub account username.

5. Set the repo to Public.
6. Go to `Setting` > `Pages`
7. Under `Build and deployment` > `Branch` > select `Main` > Click `Save`. This will trigger an automatic action to deploy and publish your website. 

8. Go to `GitHub Actions`. Once the `pages build and deployment` action is compelted and turns green, open a new tab and type `<<github_user_name>>.github.io` in the address bar.

***Congratulations you just published your site to the world-wide-web.***

To complete the setup let's add a few details to your landing page.

## Setup the landing page

To make changes to the content of your landing page we need to edit the `_conig.yml` file in the code.

### Steps

1. Navigate back to the `Code` section of your repo and click on the `_config.yml` file. Click on `Edit file in place`. You can now edit the contents of this file right in your browser.
2. Site display name: Edit the configuration parameter called 'title'.
    Eg:
3. Setup the tagline: A short punchy description of 
4. Social media handles: Update the links to your socials and email address.
5. Logo: This 

There are plenty of other options avilable to include features like comments and web page analytics. You can explore the Chirpy and [`Jekyll`](https://jekyllrb.com/docs/) documentation to learn more.

## Write your first post

Posts for your Jekyll website should reside in your `_posts` folder.

1. Navigate to the `_posts` folder in your code repo. Create a new file by selecting `Add file` > `Create new file`.
2. Set a name for your file. Ideally following this format **`YYYY-MM-DD-TITLE.md`**. The md file extention indicates that this is a markdown file. Markdown is a markup language that uses plain text to indicate formatting. It is easy to learn, click here for a reference.
4. Every post must start with a block of text called [Front Matter](https://jekyllrb.com/docs/front-matter/). 

Format of the Front Matter:
```yaml
---
title: TITLE
description: Setup and publish a blog directly from your browser in under 10 mintues!
date: YYYY-MM-DD HH:MM:SS +/-TTTT
categories: [TOP_CATEGORIE, SUB_CATEGORIE]
tags: [TAG]     # TAG names should always be lowercase
image:
  path: ../assets/img/picture.png
  alt: Alternate caption for your image.
---
```

Here:
* title: Refers to the title displayed on the broswer tab and in the sidebar on the landing page.
* description: A short para describing contents of the post.
* date: Specify the date and time of publishing.
* categories: Categories under which to group multiple posts.
* tags: Tags for the article. 
>Note: Tage names must be in lowercase and separated by commas {: .prompt-info }

5. Add some text: Use # to indicate a H1 heading
Write some paragraphs below.

6. Same the file: Click on commit to code to save the file.

**Navigate back to actions, and once deployment is successful refresh the page to reveal your first post on your new website!**

There are plenty of other types of content you can insert into your blog including images, inline video (including videos from Youtube), ordered lists, audio etc. Do take a look at the code of [this post](https://chirpy.cotes.page/posts/write-a-new-post/) on the original Chripy repo to replicate some of these elements on your own site.


*Hope you found this helpful! Do [`write to us`](mailto:mpriyanka1800@gmail.com) with any feedback/suggestions.*
