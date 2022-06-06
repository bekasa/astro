---
layout: '../../layouts/Post.astro'
url : '/blog/why-use-ssl'
tags: "blog"
pageTitle: "SSL and why use it - meteorwebsitedesign.com"
article_title: "SSL/TLS security encryption and why use it"
description: "SSL (Secure Socket Layer) is the means of encrypting data between server and web browser and free certificates are now available."
categories: "security"
pa_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1577551569/mailbox_new_bc2iq5.jpg"
pa_s_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1577551569/mailbox_new_katdde.webp"
panel_summary: "Several years have passed since Google stated their intention to encourage HTTPS everywhere. All Google services have been changed over to HTTPS along with highly trafficked sites like Facebook."
panel_image: "https://res.cloudinary.com/bekasa/image/upload/v1547300219/mailbox_kbct76.webp"
panel_image_s: "https://res.cloudinary.com/bekasa/image/upload/v1547300219/mailbox_sj_jxuelm.jpg"
panel_title: "TLS / SSL Why It is Used"
blog_image: "https://res.cloudinary.com/bekasa/image/upload/v1485807456/ssl-comp_ycoppv.png"
breadcrumb: "SSL/TLS"
date: "2017-01-28T11:00:00"
---
Several years have passed since Google stated their intention to encourage HTTPS everywhere. All Google services have been changed over to HTTPS along with highly trafficked sites like Facebook.


 Google has given encouragement to webmasters  by indicating that it is a ranking signal. Only a lightweight signal but, one that could strengthen to further encourage the trend. And in these days of imperative SEO who could resist the possibility of gaining an edge over competitors.

### What SSL/TLS is
SSL and TLS (Secure Socket Layer and Transport Layer Security) are both cryptographic protocols used in generating secure exchange of information between server and browser. TLS is used more often than not and SSL the forerunner, initially invented by Netscape. This particular aspect of website security has become commonly known as SSL. 

Current implementation is TLS 1.2 and version TLS 1.3 is under discussion. Version 1.3 will take into account existing vulnerability issues increase security still further.

### Web Browser SSL/TLS Indicators
Modern web browsers include TLS (SSL) technology and would indicate the presence of a secure data interchange session by displaying a green padlock to the left of the Internet address. And starting the Internet address with http**s**://.

![https://](https://res.cloudinary.com/bekasa/image/upload/v1485807456/ssl_icon_fvy6ga.png)

In the very near future ( around January 2017) browsers are going to display site *insecurity*. Google Chrome 56 will display the fact that the page is insecure where the page is login or requesting credit card information.
![Chrome insecure](https://res.cloudinary.com/bekasa/image/upload/v1485964718/not_secure_chrome_pjga6l.png)

Firefox displays in a slightly different way
![Firefox insecure](https://res.cloudinary.com/bekasa/image/upload/v1525961459/not_secure_yc2vwm.jpg)

Eventually, all plain HTTP pages will be flagged as non secure.
[see Google security article](https://security.googleblog.com/2016/09/moving-towards-more-secure-web.html)

### Why Use SSL/TLS?
The problem with standard Internet protocol (Hypertext Transfer Protocol **HTTP**) is that information is transferred between server and browser in cleartext format. After all, the World Wide Web was initially designed to disseminate information publicly. At any point in the delivery chain, data can be intercepted, interpreted, content altered or injected relatively easily. Particularly important with mobile devices being used on public networks.

It has been only too well reported on the press that inadequate shielding of sensitive information can lead to fraudulent financial transactions, identity theft and many more scams from data pilfering. Data thieves are becoming ever more devious and cunning and are only too well aware of public inertia around regularly changing, using secure and different passwords for each website. Often people tend to use the same passwords between sites and the data thieves exploit this and use purloined login resources in multiple intrusion attacks.

### Why Obtaining and Using SSL/TLS Certificates Have Changed
Until relatively recently, SSL certificates were used exclusively by upper echelon e-commerce and banking sites. It seemed unwarranted to consider SSL for a simple website that had no or little interaction with users. Cost of certificates and complexity were prohibiting factors.

The three factors that have allowed SSL to become more common place are, public concern with website security and privacy, the falling cost of certificates and Google intending to make the Web a safer place.

1. Public awareness, there is expectancy to see browser indication of secure browsing in use.
2. Browser manufacturers are indicating when secure connections are available.
3. Web pages can load faster  using HTTP/2 with TLS encryption.
4. Google has made plain that sites not using TLS will be penalized in some way. Initially where pages collect user information and are not using TLS. 

## How SSL/TLS Is Implemented
Both modern servers and browsers have all the necessary software to implement secure connections between the two. There is just one element missing. To actively engage SSL/TLS, a certificate is required from a **'Certificate Authority'**.

### Certificate Types
There are now free and commercial certificates available. Within the commercial area there are different types of certificate. Which one may be required depends on the use case. The broad categories of certificates available are:
1. Domain only validation and usually covers base domain eg. example.com and the www sub domain eg. www.example.com. Can be free or minimal charge of around $10 per/year. There is no difference in the quality of encryption where the certificate is free.
2. Organisation Verification 
3. EV (Extended Validation) certificates where as the name suggests more extension validation of the business and not just the domain is involved.

There are variations for multiple domains and specialist environments, the precise attributes depend on the issuing authority. Wild card certificates take the form of *.example.com are used for top level sub domains eg anything.example.com

 Commercial certificates offer financial guarantees  which cover direct losses as a result credit card transactions where a certificate has been miss-used.

Certificates are usually issued for a defined term which may range from days to years depending upon the initial purchase terms.

## Moving from HTTP to HTTPS
While the acquisition of SSL certificates has become much easier. There is still resistance to making the switch unless it becomes necessary as in the case of Facebook. One reason for this is the uncertainty around how search engine rankings will fluctuate. Undoubtedly there will be an impact, probably detrimental at first. Website pages served via http and https are considered different resources and capable of being indexed separately which could lead to duplicate content penalties.

Google recommends planning ahead before making the change 

1. 301 redirects
2. hsts headers
3. canonical tag


## SSL/TLS Certificate Acquisition
The procedure for acquiring and implementation of a certificate depends on how the website is hosted and with what company.
Site can be tested using [Qualys SSL Labs tool](https://www.ssllabs.com/ssltest/)

### Shared Hosting
There are a few shared hosting companies have that have integrated "Let's Encrypt" into their control panels. In which case, a SSL certificate can be installed easily in a couple of mouse clicks at zero cost.

With other hosts what is and is not possible and the quickest route to certificate installation depends on what the host is willing to allow. In some cases a certificate may have to be purchased through the company. It may also be a requirement to acquire (and pay for) a separate IP address. A separate IP address is not a technical necessity of a certificate, but the server configuration.

If independent purchase and installation is possible then a certificate has to be purchased (see below some for Certificate Authorities). It can be purchased and activated later.

To activate the certificate it is necessary to generate a signing request. This facility is usually available via the domain control panel and is certainly available on cPanel under 'SSL/TLS'. Just click on "Generate an SSL certificate and Signing Request" and fill out the form.
Copy the generated request and paste into the CSR space when you begin activation with the SSL provider. The final certificate is returned by email to the domain email address specified.

The remaining step is to install the certificate and is easily done from "Install an SSL Certificate" area on cPanel. Paste the certificate into the space provided and submit the form - that is all. The domain should can now use the https protocol and the site can be tested. See tests

Just because a site can use https does not necessarily mean that it will for all connections at all times. Much depends on the software employed in generating the site. It may be necessary to force https by adjusting the site configuration and or .htaccess file where applicable.

### VPS and Dedicated Server

Common server configuration files can be found at [Mozilla SSL Configuration Generator](https://mozilla.github.io/server-side-tls/ssl-config-generator/)



### Certificate Authorities

Notably, free (domain validation only) certificates are now available from [Let's Encrypt](https://letsencrypt.org/) which is a certificate authority. Certificates are valid for 90 days but, there is an automatic renewal service.

Certificate costs are usually expressed yearly but there is a wide variation of costs related to business validation and validity periods. As with any service it pays to search for alternatives. Here is a short list to to use as a starting point.

Some commercial certificate authorities:

1. sslmate.com
2. thesslstore.com
3. namecheap.com
5. comodo.com
4. goddady.com
6. ssls.com
7. networksolutions.com
8. globalsign.com
9. trustico.com
10. tartssl.com
11. sslauthority.com
    




