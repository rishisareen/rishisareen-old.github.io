---
layout: post
title: "Building Website - Part 2 - Creating New Posts"
date: 2020-09-06 13:49:45 +0530
comments: true
categories: website
---

In [Part 1](https://rishisareen.com/website/creating-website-from-scratch.html), I showed how to create a new website. In this part, we focus on how we write new articles in the website. 

## Step1 : Download Typora (Windows / Mac)

The website made in Jekyll all uses a language called Markdown to compose the articles. You don't need to understand Markdown though. There is a beautiful software [Typora](https://typora.io/). It is markdown writer, you write as you write in MS Word, and it converts it to Markdown as you write. 



## Step 2 : Copy a sample Markdown File locally from Github 

1. Go to the repository you created in Part 1 github.com/<yourusername>/<yourusername>.github.io/
2. Go to folder _posts
3. Copy a sample markdown file, or download the [file from here](https://github.com/daattali/beautiful-jekyll/blob/master/_posts/2020-02-28-test-markdown.md)



## Step 3 : Edit the Markdown file in Typora

1. Post file name should be in format YEAR-MONTH-DAY-title.md

2. Every post has header, which is meta-data. Update title and date

   ---
   **Raw Format**

   ```markdown
   --- 
   layout: post
   title: "MAF Method - Part1"
   date: 2019-03-10 02:46:16 -0400
   comments: true
   categories: running
   ---
   ```

   **As seen in Typora**

   ![](../assets/img/website-design/markdown-layout.JPG)

3. **Content**

   You can add text, image, table. Basically, anything you can do in MS Word, you can do here. Playing around is the best way to learn on this.



## Step 3 : Save the file back in Github

1. Browse to your github repository github.com/<yourusername>/<yourusername>.github.io/_posts

2. Drag the created file here

   Voila, your new post is ready. It will appear in 1-2 minutes on <yourusername>.github.io, and custom domain too



## Pending Parts

1. How to save the images in GitHub
2. Advanced Users - How to use the GitHub desktop
