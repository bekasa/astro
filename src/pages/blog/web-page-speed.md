---
layout: '../../layouts/Post.astro'
url : '/blog/web-page-speed'
tags: blog
categories: "general"
pageTitle: "Fast Website Page Loading - meteorwebsitedesign.com"
article_title: "Fast Page Loading"
description: "High performance websites load quickly, avoid user abandonment and improve conversion rates"
pa_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1577553371/speed_new_s7c3kj.jpg"
pa_s_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1577553371/speed_new_fikxfd.webp"
panel_summary: "It does not take much research to reveal that decreasing load times leads to higher conversion rates, whatever the activity."
panel_image: "https://res.cloudinary.com/bekasa/image/upload/v1547294403/speed_vdxuze.webp"
panel_image_s: "https://res.cloudinary.com/bekasa/image/upload/v1547294416/speed_sj_u1jrii.jpg"
blog_image: "https://res.cloudinary.com/bekasa/image/upload/v1477933245/speed-min_ap1qpg.png"
panel_title: "Fast Page Loading"
breadcrumb: "Fast Website Page Loading"
date:   "2016-10-10T00:00:00" 
---

**All evidence suggests that fast page loading is beneficial: there is no evidence against it. Whatever site visitors want to do, they want to do it quickly!**

Here are a few simple things that anyone can do to improve page loading speed.

Read one example of the Mozilla experience [mozilla1](https://blog.mozilla.org/metrics/2010/03/31/firefox-page-load-speed-part-i/) and [mozilla2](https://blog.mozilla.org/metrics/2010/04/05/firefox-page-load-speed-%e2%80%93-part-ii/)

##  The Tools For Testing Page Load Speed

Google is promoting "Make the Web Faster" and has provided a few tools for the purpose.
Anyone can visit [PageSpeed](https://developers.google.com/speed/pagespeed/insights/) type  a URL in the space indicated, hit return and the user will be rewarded with a score out of 100 and a list of passed and failed rules. There is also a score for user experience for mobile devices. Solutions and suggestions are also offered.

There are a similar tools at 

1. [Pingdom](https://tools.pingdom.com/), and there is an option to test from various locations.
2. [Webpagetest](https://www.webpagetest.org/) and
3. [Gtmetrix](https://gtmetrix.com/)


### Tested Parameters

All the above tests have similarities some are more detailed and have different emphasis.

Taking Google Page Insights as an example, the tests are focused on these elements. 

1. Reducing server response time.
2. Optimize images.
3. Minify Html and Page compression.
4. Avoiding landing page redirects.
5. Prioritize visible content.
6. Minification of stylesheets and JavaScript. 
7. Remove render blocking stylesheets and JavaScript.
8. Browser caching.


## Speed Test Solutions

The Google insights test will not only list errors but make suggestions on fixing issues and even provide file resources which can be downloaded and implemented.

The first three items in the following list are things that the most non technically minded can easily undertake.

### Reducing Server Response Time

The solution is straight forward, if the current hosting arrangement is inadequate change the host for a better one.

### Optimizing Images

The objective is to reduce image file size without appreciably degrading the quality of the image. Thereby allowing faster download and browser render times and saving valuable and possibly costly bandwidth. Most web applications do not require high definition images and usually it is a waste of resources to use them. 

Of the three common file types PNG, JPEG and GIF, as a rule of thumb it is usually better to us a .jpg (or .jpeg they are the same). The level of detail under most circumstances is better and they are able to be compressed considerably. They are the de facto standard of the web.

#### Image Editing

The first step is to optimize the image *dimensions*. There is no point in incorporating 1200 px * 800 px images if only 600 px * 400 px images are utilized. On the other hand it  is counterproductive to use images which are too small because they will appear distorted.

Image editing and compression are features of image manipulation programs Adobe Photoshop and [GIMP](http://www.gimp.org/). GIMP is an open source project and is free to download and use and can be run on Windows, Mac or Linux.

Online image editing is available with [FotoFlexer](http://fotoflexer.com/).

#### Image Compression

If no image editing is required, there are some quick and easy image compression services available.

A search for "online image optimizer" will reveal numerous services which will complete the file size reduction process ([Optimizilla](http://optimizilla.com/), [ImageOptimizer](http://tools.dynamicdrive.com/imageoptimizer/)] are just two of many).


### Page Compression

Most often  hosting providers will have an option to "optimize" a website and when activated site files will be compressed. Using this option is usually very simple and just involves clicking on an icon.

![optimize website](https://res.cloudinary.com/bekasa/image/upload/v1476967138/opimize-website_gqda7q.png)

The screen that follows will offer a list of file types to be processed choose the all files option.

### Minify Style Sheets and JavaScript

Combining multiple style sheets and scripts does require a certain level of expertise. The end result is one style sheet and one script where white space has been removed. Usually there are significant file size reductions.

How to complete this exercise depends on how the website is generated. 

1. Static site will probably require setting up an asset pipeline and incorporating that in the build process.
2. If one of the popular site generation programs have been used like Wordpress or Joomla there are either incorporated solutions or plugins available for the purpose.

For Wordpress there are several cache plugins which will automate the process to some extent although some configuration may be required. Top rated Wordpress plugins are [W3 Total Cache](https://wordpress.org/plugins/w3-total-cache/), [WP Super Cache](https://wordpress.org/plugins/wp-super-cache/), [Wp Fastest Cache](https://wordpress.org/plugins/wp-fastest-cache/) and [ZenCache](https://wordpress.org/plugins/zencache/).

### Removing Render Blocking Stylesheets And JavaScript

This is a more testing requirement. The often advocated solution for the JavaScript file is the place it at the end of the page just before the close of the body tag. In that way the scripts are called when the page has been rendered.

Dealing with the style sheets is more of a conundrum because the requirement is circular. The page cannot be rendered unless the browser knows how to do so but yet the style sheet prevents rendering until it has been loaded.

The two basic solutions are one incorporate styling inline with the page and two load the style sheet asynchronously. Neither one is easy to implement without some technical knowledge.

## Conclusion

With relatively simple actions page speed can often be improved considerably, even by the non technically minded. The results attainable vary but, with a responsive layout, good quality hosting, image optimization and the use of caching plugins or components will improve page speed scores. 

In some instances top score of 100 will not be possible but scores in the high 80's and low 90's are an attainable target.
