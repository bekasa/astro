---
layout: '../../layouts/Post.astro'
setup: |
  import Tick from '../../components/Tick.astro'
url : '/blog/confidential-email-services' 
tags: blog
pageTitle: "Confidential (Encrypted) Free Email Services in Europe - meteorwebsitedesign.com"
article_title: "Free Tier Encrypted Email Services"
description: "Major benefits of using one of the free tier confidential (encrypted) email services in Europe"
categories: "general"
lead: "Email Service Providers"
pa_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1577548332/pidgeons_vppywm.jpg"
pa_s_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1577548344/pidgeons_nkxafl.webp"
panel_summary: "Confidential email Services"
panel_image: "https://res.cloudinary.com/bekasa/image/upload/v1548957138/flying_pidgeons_z5pwpf.jpg"
panel_image_s: "https://res.cloudinary.com/bekasa/image/upload/v1548957138/flying_pidgeons_s_ouvktn.jpg"
blog_image: "https://res.cloudinary.com/bekasa/image/upload/v1549836671/clock-padlock_cr_a6k3lv.png"
panel_title: "Confidential Email Services"
breadcrumb: "email providers"
date:   "2019-02-05T11:00:00" 
---
## Public Nature of Email Services
This article is about raising awareness of the current general level of email privacy and security and the tools to easily engage with confidential emails. Also demonstrating that it can be very advantageous to consider email and document encryption and how it can be done painlessly. This is not a shield for nefarious activities, the major benefits are reducing exposure to privacy law liability and bolstering client confidence.


It should be understood at the outset that the Internet is a very public medium, privacy and security of information cannot be taken for granted at any level. Popular online email services (Gmail, Yahoo, Yandex etc.) do not encrypt documents at rest with the potential for compromise of your privacy and that of associates.

It must also be assumed from the outset that the provision of **'free'** services are being monetized somehow and that somehow is often by selling, in some form, data acquired. None of the service providers are charitable organisations. The user and their data have become the **product** for sale.

Privacy threats are very real, data breaches are now a very common occurrence which underlines just how difficult it is to maintain a **'secure'** online environment. This is quite apart from backdoor access granted to NSA and other security agencies. Consequent punitive fines levied after the genie is out of the bottle are of little use or consolation. 

For all these and many more reasons it could be wise to consider mail and document encryption under some circumstances or, at least becoming familiar with technologies and services  available  now. 

### Securing Emails At Rest By Encryption
There may be occasions when the necessity of personal, sensitive or private information collection arises in the natural course of business activities.
Many jurisdictions impose a duty of care that information of this private nature is collected and stored by the most appropriate and secure means. This is especially true in Europe now that the General Data Protection Regulation (GDPR) became enforceable from 25 May 2018. 

Email is without doubt the most common form of communication but, it did not originate with any thought of privacy. Email is a simple protocol with no intrinsic security attributes. Messages are passed around the Internet in plain text, and without any safeguards can be intercepted and read.

The biggest general privacy upgrade in recent times has been the adoption of SSL/TLS encryption on a wide scale. Google being a major player in it's promotion. Mail in **transit** is therefore better protected against interception to the extent that SSL/TLS has been implemented. Although a great improvement, SSL/TLS alone is not absolutely bullet proof.

 Major privacy and security issues arise with emails at rest, that is mail deposited in an inbox awaiting collection or reading. Most popular email service providers emails are not encrypted although they all use transit encryption.

**End to end encryption (E2EE)** is the only way to ensure that emails cannot be read except by authorised parties. Documents are encrypted before they begin transit and are decrypted by the end user after transmission.


### Email and Document Encryption

The most popular method of encrypting documents is by OpenPGP standard and there are several flavours of implementation. The process involves the generation of paired keys which are mathematically related. Key generation is specific to one email address.

The public key can be made widely available by using keyring servers or even sending along as an attachment with an email. Decryption is then undertaken by the recipient with the private key. 

Most operating systems provide means for using the OpenPGP standard but for the average user this will prove complex and confusing. Gaining proficiency in use would take some research and practice. In some instances it would probably be necessary to use the console or terminal, which is outside most users' comfort zone. 

There are simpler options like **'Malevelope'**  and **Flowcrypt** browser add ons available for Google Chrome and Firefox. It makes key administration much easier but probably not convenient enough to encourage mainstream usage.

### Email and Document Encryption Solutions
There are already available mail services that embrace encryption and privacy. Some which offer a free service tier are listed below. All these are on the European side of the pond which makes good sense for a multitude of reasons especially with GDPR.

These services store documents in encrypted form in secure locations. Most insist that they cannot read stored materials. 

Users having accounts with the same service can exchange encrypted mail invisibly just like any plain text service. Encryption and decryption is carried out seamlessly.

### Interoperability Between Encrypted and Plain Text Email Services
Methods of interfacing encrypted and non encrypted services are available and easy enough for anyone to use. Sending an encrypted message from one of these services is simply writing the message and setting a password. The password has to be transmitted by another channel (also with end-to-end-encryption) **'Signal'** for instance.

The recipient receives notification that a confidential message has been sent to them along with a link for reading. After entering the pre-arranged password the message can be **read and replied to**.


## Confidential Email Providers

### Mailfence


<img src="https://res.cloudinary.com/bekasa/image/upload/v1549815171/mailfence_c_l6pijs.png" alt="mailfence"/>

Probably the most extensive service listed here including both paid and free tiers. Paid options begin at a very reasonable 2.5 &euro; / month. Services increase dramatically with email storage rising to 5 GB, support included, Imap, POP, SMTP's available along with custom domains.

The free tier includes options to upload, store and manage  PGP keys. Either outward bound mail can be encrypted by password or key. In the case of password protection, notification of the email is sent. After entering the password, the encrypted mail is displayed along with the option to reply.

Emails can be set to destruct from one week upwards or never.

This document store allows uploading and organisation of documents.

Calendar events and notifications are available.

Mailfence Features

* <Tick></Tick> Includes 500 Mb of email storage
* <Tick></Tick> Includes 500 Mb of document storage
* <Tick></Tick> Open source cryptography
* <Tick></Tick> Includes end-to-end-encryption and complete privacy
* <Tick></Tick> 2FA (Two Factor Authentication) available
* <Tick></Tick> Auto destruct emails
* <Tick></Tick> Secure data centre in Belgium
* <Tick></Tick> 1000 calendar events
* <Tick></Tick> Clear documentation

### Tutanota


<img src="https://res.cloudinary.com/bekasa/image/upload/v1549801447/email_panel_c_dpdvhx.png" alt="tutanota"/>

'Tutanota is the world's most secure email service' to quote their propaganda is the German offering in this arena. Certainly a clean and efficient minimal workspace. There is all that is needed but no clutter with toys and distractions that are not.

The openPGP standard is not followed, instead a hybrid encryption scheme is used so 'key sharing' is not possible. Encrypted mails include subject, content and attachments, some email metadata (sender, recipient, date) is not encrypted.

Mail between Tutanota users is fully encrypted and then stored. However, mail may be sent to other email services as either plain text or as a 'confidential' email. In the latter case, an invitation to read the mail is issued. After entering a pre-arranged password, the recipient has access to the mail in a 'virtual' mail inbox.

One of the greatest weaknesses with password security systems is password reset by email. Easily exploitable and used often to allow password resetting of user related accounts. Tutanota avoids this pitfall by generating a recovery code when the account is initiated and is available from the admin panel when logged in to the system. If password and recovery code are both lost then the account becomes inoperable. Tutanota cannot gain access because they do not store the decryption keys.

This is an ideal system for those beginning with confidential emails and who have more questions than answers. There is no fiddling around with keys or any other paraphernalia. Simply write the email include any attachments and send - job done.

Tutanota Features

* <Tick></Tick> Includes 1 Gb of email storage
* <Tick></Tick> Open source cryptography
* <Tick></Tick> Includes end-to-end-encryption and complete privacy
* <Tick></Tick> 2FA (Two Factor Authentication) available
* <Tick></Tick> Apps available for Android, iOS
* <Tick></Tick> Anonymous signup
* <Tick></Tick> Secure data centre in Germany
* <Tick></Tick> Subscription allows private form processing
* <Tick></Tick> Clear documentation


### Protonmail

<img src="https://res.cloudinary.com/bekasa/image/upload/v1549813477/protonmail_sde1tr.png" alt="protonmail"/>

If there is concern for security and privacy this provider has servers based in Switzerland should be given serious consideration. It boasts servers physically located below 1000 metres of solid rock. Compliance with Swiss very strict privacy laws and as an added bonus the limited potential for data leakage helps immensely with European General Data Protection Regulation (GDPR) compliance. Although Switzerland is not a member of the European Union.

Access to protonVPN is available to free users.

Protomail Features

* <Tick></Tick> Includes 500 Mb of email storage
* <Tick></Tick> Open source cryptography
* <Tick></Tick> Includes end-to-end-encryption and complete privacy
* <Tick></Tick> 2FA (Two Factor Authentication) available
* <Tick></Tick> Apps available for Android, iOS, Web
* <Tick></Tick> Anonymous signup
* <Tick></Tick> Secure data centre in Switzerland 
* <Tick></Tick> Clear documentation
* <Tick></Tick> Access to protonVPN

## Can't Live Without My Gmail, Yahoo etc.

If after looking over the above offerings and come to the conclusion that you still prefer to stick entirely with those services then one option is to use a browser add-on like **Mailvelope** or **Flowcrypt**. Be aware that using these options requires a clear understanding and good organisation or mayhem can ensue. 


### Conclusion

Both Tutanota and Protonmail are well respected and considered to be at the top of the confidential email services tree. Both deal with their main objectives very well but they are of necessity very much feature restricted when compared to popular mail services. For instance, searching mail is more limited because at a minimum the body of all mails is encrypted.

All the encryption in the world is not going to be of any value if passwords are not duly generated and secured.

### References

Confidential email services

[Mailfence](https://mailfence.com)

[Tutanota](https://tutanota.com)

[Protonmail](https://protonmail.com)

End to end message encryption

[Signal](https://signal.org/)

Online password Generators

[Strong Password Generator](https://strongpasswordgenerator.com/)

[Last Pass](https://www.lastpass.com/password-generator)

<hr />
