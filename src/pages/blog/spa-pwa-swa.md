---
layout: '../../layouts/Post.astro'
url : '/blog/spa-pwa-swa'
tags: blog
pageTitle: "Single Page App. (SPA), Progressive Web App. (PWA), Static Progressive Web App. (SPWA) - meteorwebsitedesign.com"
article_title: "The Core Ideas About SPA's, PWA's, SPWA's"
description: "Definition and differences between Single Page App. (SPA) Progressive Web App. (PWA) or a Static Progressive Web App. (SPWP)"
categories: "general"
lead: "What type of website am I."
pa_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1579803874/question_s_uyhkkm.jpg"
pa_s_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1579803874/question_otcu4t.webp"
panel_image: "https://res.cloudinary.com/bekasa/image/upload/v1548263749/question_dktqdy.jpg"
panel_image_s: "https://res.cloudinary.com/bekasa/image/upload/v1548263749/question_s_m5t7s8.jpg"
panel_summary: "Definition and differences between Single Page App. (SPA) Progressive Web App. (PWA) or a Static Progressive Web App. (SPWP)"
blog_image: "https://res.cloudinary.com/bekasa/image/upload/v1548602438/question_i3svs7.png"
panel_title: "About SPA's, PWA's, SPWA's"
breadcrumb: "What am I"
date:   "2019-01-27T11:00:00" 
---
A short article hopefully bringing clarity to the some confusing terms such  as SPA, PWA, SPWA.

### Single Page Application (SPA)

So-called because to all intents and purposes there is only one apparent page, the landing page. The layout remains the same and only content is changed.
Content is changed by server request and a new 'page' rendered. Very efficient, because only the content is rendered or re-rendered not the whole document.

Today, popularized by modern frontend JavaScript frameworks like **React**, an app is usually built as a single page application: you only load the application code (HTML, CSS, JavaScript) once.

SPA's are best consigned to applications rather than building websites that require SEO because although search engines clever as they may be, do not interpret Javascript and cannot easily distinguish 'pages' for indexing and ranking purposes. Common example of an SPA would be Gmail.

Main advantage of an SPA is that it appears very fast to the user much like a desktop application. SPA's are easy to transform into Progressive Web Apps, which in turn enables the provision local caching and to support offline experiences.

### Progressive Web Application (PWA)

To quote Google developer 

A Progressive Web App is:

* **Progressive** - Works for every user, regardless of browser choice because it's built with progressive enhancement as a core tenet.

* **Responsive** - Fits any form factor: desktop, mobile, tablet, or whatever is next.

* **Connectivity independent** - Enhanced with service workers to work offline or on low-quality networks.

* **App-like** - Feels like an app, because the app shell model separates the application functionality from application content.

* **Fresh** - Always up-to-date thanks to the service worker update process.

* **Safe** - Served via HTTPS to prevent snooping and to ensure content hasn't been tampered with.

* **Discoverable** - Is identifiable as an "application" thanks to W3C manifest and service worker registration scope, allowing search engines to find it.

* **Re-engageable** - Makes re-engagement easy through features like push notifications.

* **Installable** - Allows users to add apps they find most useful to their home screen without the hassle of an app store.

* **Linkable** - Easily share the application via URL, does not require complex installation.

So, with that definition fairly simple websites can become a PWA. But they would need a couple of extra ingredients to make them behave in the prescribed way. Firstly, a manifest file has to be generated which details information about the app and then the installation of a Javascript 'service worker'.

A service worker task operates in the background and does not interfere with user interaction. It's function is to cache necessary assets including  document pages. This caching process gives the app the appearance of speed because network access is not necessary. The overall impression is one of a native desktop app rather than a web based app.

### Static Progressive Web App (SPWA)

So called because they undertake to remove the primary weakness of the SPA, the difficulty with SEO and search engine indexing. And they do that by generating static pages which have their own meta data, title and description etc.

Several frameworks are appearing that generate static pages in this manner and possibly the most popular (at the time of writing) is GatsbyJS. Truly impressive since it not only generates these vital static pages but also make use of graphQL technology for sourcing data.

Using graphQL for data sourcing is one of the outstanding features of GatsbyJS because it allows any source that has a graphQL server to become a data source in addition to local files.

Navigating a GatsbyJS site becomes almost instantaneous from the outset ten pages are included with the initial landing page load. The only downside to that is the the initial loading can be on the slow side.


### References

[Google explanation of PWA](https://developers.google.com/web/fundamentals/codelabs/your-first-pwapp/)

[Gatsby a Static Progressive Web App Framework](https://www.gatsbyjs.org/)
<hr />
