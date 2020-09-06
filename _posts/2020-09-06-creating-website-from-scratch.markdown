---
layout: post
title: "Building Website from Scratch in 30 min"
date: 2020-09-06 13:49:45 +0530
comments: true
categories: website
---

I recently built a website from scratch for a friend. This article captures my notes.



## Step1 : Deciding on the Framework

First step to build a website is to clearly define the goal. That will help to arrive at the framework choice.

In this case, goals were:

1. **Blogging** : Prime purpose of building this website was to write articles. 
2. **Support of Custom Domain** : Your website is your identity on the internet. Having a custom domain just looks more professional.  And with cost under INR 1000/- per year, there is no reason not to have a custom domain. 
3. **Ease of Operation** : My friend, though super smart, is not from Software field. Ease of daily usage was crucial. 
4. **Low Recurring Cost** : As it was a blog based website, with a potential hit of 10k subscribers in first year, focus was not to spend extra money on complicated domain based hosting.

With all these goals, I picked 

1. **Framework** : [Jekyll](https://jekyllrb.com/) with Theme [Beautiful-Jekyll](https://github.com/daattali/beautiful-jekyll#readme)

   **Jekyll Advantages**

   - Effortless to use
   - Create Static Websites - so website is lightweight, rapid to load
   - Free Software
   - Supported by GitHub pages. 
   - Multiple Themes supported. So website look can be customized quickly. 

2. **Hosting** : [GitHub Pages](https://pages.github.com/)

   - Free to use for personal websites
   - Support for Custom Domain
   - Support for https

3. **Domain Registrar** : [Google Domains](https://domains.google.com/)

   - Clean Interface, less spammy  than GoDaddy.



## Step 2 : Creating Website

We will be creating and storing the website on [GitHub](https://github.com/). We will be copying a pre-existing theme and customize it as per our need.

Scroll down to see the steps involved, but here is a 40-second video just as a reference as you work through the steps. 



![Installation Steps](../assets/img/install-steps.gif)

1. ### Create login on [GitHub](https://github.com/)

2. ### Fork the Beautiful-Jekyll theme 

   Fork this project by going to https://github.com/daattali/beautiful-jekyl and clicking the ***Fork\*** button at the top right corner of this page. Forking means that you now copied this entire project and all the files into your account.

3. ### Rename the project to `<yourusername>.github.io`

   Click on ***Settings*** at the top (the cog icon) and on that page you'll have an option to rename the project (*Repository name*). This will create a website with the **Beautiful Jekyll** template that will be available at `https://<yourusername>.github.io` within a couple minutes.

4. ### Customize your website settings

   Edit the `_config.yml` file to change any settings you want. To edit the file, click on it to view the file and then click on the pencil icon to edit it (watch the video tutorial above if you're confused). 

5. ### Congratulations! You have a website!

   After you save your changes to the `_config.yml` file (by clicking on *Commit changes* as the video tutorial shows), your website should be ready in a minute or two at `https://<yourusername>.github.io`. Every time you make a change to any file, your website will get rebuilt and should be updated in about a minute or so. Your website will be initialized with several sample blog posts and a couple other pages.



## Step 3 : Buying Domain

1. Go to [Google Domains](https://domains.google.com/registrar/search)
2. Search for the domain name. 
3. Fill the details. 
4. Purchase

That's it. It is as simple as it sounds. 

A small video for your reference

![Getting New domain](../assets/img/google-domains-registrar-choosing-domain-name.gif)



## Step 4: Redirecting New Domain to Github Pages

In this step, we redirect our newly created domain to GitHub pages. For this we need to do 2 steps

### 1. Let GitHub Pages know your custom domain

1. Go to your github repository settings page

   ![](../assets/img/website-design/github-settings.png)

2. Add you custom domain name at Settings > GitHub Pages > Custom domain

   ![](../assets/img/website-design/github-github-pages.png)

   ### 2: Let your custom domain point to GitHub Pages

   1. Go to [registar](https://domains.google.com/m/registrar/) page on your google domains, select your domain

      ![](../assets/img/website-design/google-domain-list.png)

   2. Go to DNS > Custom resource records

      ![](../assets/img/website-design/google-domain-custom-resource.png)

   3. Add the record shown in the screenshot bellow. Note that you need to use the "+" button to add more urls.

      ![](../assets/img/website-design/google-domains-a-record.png)

      Here is the list of ips in the screenshot:

      - 185.199.111.153
      - 185.199.110.153
      - 185.199.109.153
      - 185.199.108.153

   4. Add the following CNAME record to point your custom domain to GitHub Pages

      ![](../assets/img/website-design/cname-record.png)



That's it. The custom domain is set up and live! 