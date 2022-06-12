---
layout: '../../layouts/Post.astro'
url : '/blog/restic-and-duplicati'
tags: blog
page Title: "Restic & Duplicati Two Backup and Restore Options"
article_title: "Restic & Duplicati Two Backup and Restore Options"
description: "Restic & Duplicati two backup and restore options that work on multiple operating systems"
categories: "general"
lead: ""
pa_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1654747743/restic_duplicati_c_chsxpu.jpg"
pa_s_jpg: ""
panel_summary: "Restic & Duplicati two backup and restore options that work across multiple operating systems"
panel_image: ""
panel_image_s: ""
blog_image: "https://res.cloudinary.com/bekasa/image/upload/v1654747778/restic_duplicati_s_c_q4rjbo.jpg"
panel_title: "Restic & Duplicati"
date:   "2022-06-10T11:00:00" 
---

Two well known programs for backing up and restoring files. Both work with the command line, multiple operating systems including Windows, Linux and Mac. The big differnce between them is that Duplicati has a web interface which can be viewed using a browser at port 8200. So for those not comfortable with the command line (terminal) then Duplicati is a good alternative.

### Installation

**Restic**
Stable release versions are available from the <a href="https://github.com/restic/restic/releases/latest" target='_blank'> restic release page</a>

**Windows**
Resitc can be installed by scoop but it is far easier to download the binary save to a known location and set the PATH variable if necessary

**Linux**
Can for many distributions be installed by apt-get as other software or by using one of the precompiled binaries

**Mac**
Installation is available by 'homebrew'.

**Duplicati**

Downloads are available directly from the home page simply proceed as required for normal software installations for Windows
Linux and Mac. Linux installations will require additional software to function

### Using Restic

Restic is a mature, robust and well tested backup software solution. Simple to use on the command line

**Backup**
As mentioned above restic commands are used in a terminal which are easy enough even if you would prefer to use a GUI.
Restic is capable of backing up files both to connected and remote drives. The first step is to initialise a repository at the desired location. Available storage locations include local, SFTP, REST servers as well as numerous commercial providers including Google Cloud Storage, Amazon S3, Blackblaze B2, Microsoft Azure and many more.

Local storage example to drive E on Windows <code>init repo E:/path to repo/restic_backup</code>

It is required to enter a password a warning is given not to lose or forget , otherwise files stored in the repository will be irretrievable.

Backing up <code>restic -r  E:/path to repo/restic_backup --verbose backup ~/Documents</code>

The '-r' flag indicates the repository and is required, the '--verbose' flag is optional but includes additional information related to the backup. A 'snapshot' of the files is stored in the repo. Files can be excluded with the '--exclude' option either explicitly or by pattern matching.

**Restore**

Restoration is just as easy as backup and a Windows example would be. 

<code>restic -r E:/path to repo/restic_backup restore latest --target C:/path to restore directory></code>

The option 'latest' could be replaced by a reference to a specific repo which can be realised by requesting a snapshot listing.

<code>restic -r E:/path to repo/restic_backup snapshots</code>

**Delete Repo**

Backup storage is finite and for that reason snapshots will have to be removed regularly

<code>restic -r E:/path to repo/restic_backup forget cccc1234</code>

The snapshot is removed but references to it in the repository are not. To remove those references the repository has to be pruned.

<code>restic -r E:/path to repo/restic_backup prune</code>

The operation can be combined.

<code>restic forget --keep-last 1 --prune</code>

Removal policy can be organised with the '--keep-last n' flag, where n is the number of most recent snapshots to keep.

### Using Duplicati

Duplicati with the web interface is very easy to use and bound to find quick acceptance with GUI fans.
![Diuplicati](https://res.cloudinary.com/bekasa/image/upload/v1655045341/Duplicati_900_pz7ldr.webp)

When setting up a new backup the first step is to determine the backup location and the choice is between the following standard option and the following proprietory ones.

![Duplicati Settings](https://res.cloudinary.com/bekasa/image/upload/v1655045357/Duplicati_backup_settings_yysxak.webp)

**Standard protocols**
- Local Disk
- FTP
- FTP (Alternative)
- OpenStack Object Storage / Swift
- S3 Compatible
- SFTP (SSH)
- WebDAV

**Proprietory**
- B2 Cloud Storage
- Dropbox
- Google Cloud Storage
- Google Drive
- HubiC
- Jottacloud
- mega.nz
- Microsoft Office 365 Group
- Microsoft OneDrive for Business
- Microsoft OneDrive v2
- Microsoft SharePoint
- Microsoft SharePoint v2
- OpenStack Simple Storage
- Rackspace CloudFiles
- Rclone
- S3 compatible
- Sia Decentralized Cloud
- Tardigrade Decentralized Cloud Storage
- Tencent COS

After choosing a protacol if required, additional information is requested such as bucket name, application key etc.

**Selecting Backup Source**

![Duplicati Source](https://res.cloudinary.com/bekasa/image/upload/v1655045907/Duplicati_source_qsxiib.webp)




### References

<div><a href="https://restic.net" target='_blank'>Restic</a></div>

<div><a href="https://restic.readthedocs.io/en/stable/" target='_blank'>Restic Documentation</a></div>

<div><a href="https://www.duplicati.com/"  target="_blank">Duplicati</a></div>

<div><a href="https://duplicati.readthedocs.io/en/latest/" target="_blank">Duplicati Documentation</a></div>
