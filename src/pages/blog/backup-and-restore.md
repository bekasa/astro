---
layout: '../../layouts/Post.astro'
url : '/blog/backup-and-restore'
tags: blog
page Title: "Computer Data Backup and Recovery Strategies"
article_title: "Avoid Disaster with Computer Data Backup and Recovery Strategy"
description: "Data Backups and recovery plan is essential to avoid permanent loss of data, whether by catastrofic hardware failure or device loss."
categories: "general"
lead: "Backup and Restore"
pa_jpg: ""
pa_s_jpg: "https://res.cloudinary.com/bekasa/image/upload/v1628437947/backup1_kodmbl.jpg"
panel_summary: "A tested data backup and recovery strategy will pay handsome dividends should the need arise. Avoiding data loss, costly downtime and recovery after a system failure."
panel_image: ""
panel_image_s: "https://res.cloudinary.com/bekasa/image/upload/v1628358177/backup_etf9qc.jpg"
blog_image: "https://res.cloudinary.com/bekasa/image/upload/v1628358177/backup_etf9qc.jpg"
panel_title: "Data Backup and Recovery Strategies"
breadcrumb: "backup-restore"
date:   "2022-06-01T11:00:00" 
---

## Backup and Restore

Developing a rigorously *tested* software backup and restore policy for your home and / or business is not a wish list item but an absolutely crucial necessity. Should hardware or software fail a well tested policy can save sleepless nights, unnecessary expenditure, and ensure minimum downtime. 

You may sigh at the very thought of orchastrating backups but if ever the need arises to restore you will be very pleased you engaged. Even if the financial circumstances are not great the minimum expenditure should be on an external hard disk which have capacities of 3+ TB for around 100€.

Potential threats to your computing system come in both hardware and software forms. Likely sources of hardware failure are hard disks whether HDD or SSD. Software threats from malware, mail attachments, ransomware to name but a few. 

Depending on use, worthy of consideration may be the use of a **NAS** (network attached storage). A NAS is a local network connected collection of hard disks (a private cloud). The great advantage is that storege is completely under owner control. Prices differ according to capacity and capability.

Relying on just one computer is living on the edge and can make life difficult. Suppose for a moment that there is failure on the only existing machine but parts are not easily available or repair has to be carried out by a non local service centre. Or repair out weighs the cost of a new machine! With just one option getting back up and running could take a few weeks.



### Backup Location

Contigous with a general policy is the question of where to put what data. There is no rule against multiple backups  or overlapping data saved. The IT industry recommends three backups but at the very least two external hard disk and cloud for example. Data of a static nature and not likely to change, for instance pictures could be stored anywhere, locally on USB stick, external hard disk or remotely by cloud storage.

**Cloud**

Cloud storage depends on an a reliable internet connection and an equally reliable service. Services can evaporate, which leaves translating data to another location.

**Local**

Using local storage is going to be much cheaper in the long term with large amounts of data and you have complete control of the storate medium. 

**Types of Backup**

There are three basic types of backup; Full, Incremental, and Differential.

Full: A full backup backs up all the files in the back up target ( Whole disk image ).

Incremental: An incremental backup backs up all files that have changed since the **last backup**.

Differential: A differential backup backs up all files that have changed since the **last full backup** eg Restic, Duplicati. 

### Restoring Data

How restoration is undertaken is going to depend on the method used to backup.
Windows OneDrive provides a basic type of backup and stores files from Desktop, Documents and Pictures folders. Google Drive allows more choice of which folders can be backed up, which can be accessed installing <a href="https://www.google.com/drive/download/" target='_blank'>Google Drive for PC</a> . 

These are blunt tools and do not allow refinement of files to be included or excluded in a repository. This is not a trivial point since needless avoidance of duplicated or unnecessarily stored data can be avoided.

### Operating Systems

Common operating systems Windows, Linux and Mac, the methods of generating backups are generally  different although there is software available for multiple systems.

### Linux Backup and Restore methods

Linux has a rich eco system of tried and tested freely available backup software.

**Timeshift**
Intended for system backup and restore although can be set to include home directory. Bear in mind the bigger the backup the longer it is going to take to restore. Timeshift requires a Linux file system to function so if you have purchased an external hard disk it will probably be formatted with NTFS. Here is an example of commands you could use to format ext4. **Bear in mind this is just an example and you will probably need to adjust to your own setup.**

**Find the disk to re-format**

<code class="inline-block">
<div>sudo parted /dev/sda print devices</div>
<div>/dev/sda (1000GB)</div>
<div>/dev/sdb (500GB)</div>
</code>

**Create partition**

<code class="inline-block">
<div>sudo parted /dev/sbd mklabel gpt</div>

<div>sudo parted /dev/sdb mkpart primary 0% 100%</div>
</code>

**Format with ext4 file system**

<code class="inline-block">
sudo mkfs.ext4 /dev/sdb
</code>

**Deja Dup**

Uses Duplicity which in turn uses rsync, comes ready installed on Ubuntu 20.04 LTS.

**Grsync**

Graphicl interface for rsync which has the basic options, other options can be added to the command line within 'Additional options' within the 'Advanced options' tab.

**TAR** 

Terminal based but yet very popular on Unix/Linux systems, full options can be read in the manual <a href="https://www.gnu.org/software/tar/manual/" target='_blank'>here</a>. Very popular with web masters because it can copy multiple directories into one file while still preserving directory structure.

Flavours of Linux often incorporate some of the more popular software with initial installation otherwise can be installed through 'apt-get (software name) install'


## Windows 10 /11

Windows systems are notariously fickle quite apart from earlier apparitions like the '*blue screend of death*'. Linux systems on the other hand have a reputation for solid performance.
There is a good likelihood that a some stage your Windows system will misbehave in some way.

So, what does Windows 11 still does not have good backup system. Not much, it is possible to generate a system image though.

First up before doing anything obtain a copy of Windows.iso or create bootable USB this will help avoid big trouble. To do so head over to the Microsoft [download](https://www.microsoft.com/en-us/software-download/windows10?ranMID=24542&ranEAID=kXQk6*ivFEQ&ranSiteID=kXQk6.ivFEQ-h8pRcABL80vrne3eFRPakw&epi=kXQk6.ivFEQ-h8pRcABL80vrne3eFRPakw&irgwc=1&OCID=AID2000142_aff_7593_1243925&tduid=%28ir__2qlfoofp9kkfqmolkk0sohz31m2xutjtps2ustoa00%29%287593%29%281243925%29%28kXQk6.ivFEQ-h8pRcABL80vrne3eFRPakw%29%28%29&irclickid=_2qlfoofp9kkfqmolkk0sohz31m2xutjtps2ustoa00) page. Download the build tool and double click on the .exe file. A window opens to gather data and generate the requested USB or .iso file. To convert the .iso image to  bootable disk download <a href="https://rufus.ie/en_US/" target='_blank'>rufus</a>. Rufus is not 'installable' as such, simply double click on the .exe file and give permission for the program to run.

**Rufus set up screen**
![rufus screen](https://res.cloudinary.com/bekasa/image/upload/v1624216830/Screenshot_2021-06-20_210928_szsrud.jpg)


Next, timewarp back to Windows 7 at Settings > Update & Security > Backup > Backup and Restore. There is creating the system image capability which is probably the most reliable between File History or Restore Point options. And the Recovery Drive will only generate a new system sans your personal files.

System images tend to be big so an external hard disk will be required. USB flash drives curry no favour but it is possible to use DVD writer if available.

A better solution in this instnce would be Macrium Reflect 8 (see below)


## MAC

Whether you are an Apple fan or not the clarity, simplicity and ease of use of 'Time Machine' has to be admired. Every Mac arrives with Time Machine installed and available for use striaght out of the box. The decision that has to be made is where to place backups HDD, SDD, USB, Cloud etc much the same as other operating systems.

It is possible to use external (compatible) drive, USB stick, compatible NAS, another Mac computer or iDrive. If the external drive requires formatting the process is simple, note as with any format options all data will be lost.

Restoration is again made very easy, choices are individual files, multiple files or entire system.

For those looking for more specific backup, rsync (written for Unix systems and incorporated in Linux distributions) is already installed and grsync is available using brew.

**Managing Backups**

It is always good policy to backup files frequently but doing it manually can be time consuming and boring. And options like OneDrive don't allow much flexibility unless the data is kept within one the the three folders copied (Desktop, Pictures, Documents).

Backups can be organised by specialised software <a href="/blog/restic-and-duplicati" >Restic & Duplicati</a> where backup targets can be chosen from local to multiple online storage services. Backup intervals and restore location can be set or changed as required.


**References**

<u>**Cloud Storage Providers**</u>

|Provider |&nbsp;&nbsp; | Comment|
|---------| ---  |  ---  |
|<a href="https://icedrive.net/" target='_blank'>Icedrive</a>|&nbsp;&nbsp; | 10GB free of charge, clean interface, encryption available, good download speeds|
|<a href="https://mega.io" target='_blank'>MEGA</a>|&nbsp;&nbsp; |20GB+ free, good interface, encrypted, catastrophic download speeds which can drop to 0 B/s|
|<a href="https://drive.google.com" target='_blank'>GoogleDrive</a>|&nbsp;&nbsp; | 15GB capcaity shared with all other services per Google account|
|<a href="https://www.backblaze.com/"target='_blank'  >BackblazeB2</a>|&nbsp;&nbsp; |First 10GB of storage free thereafter charges apply, can be integrated with backup and restore software eg restic, Duplicati.

<u>**Windows Related**</u>

|Provider |&nbsp;&nbsp; | Comment|
|---------| ---  |  ---  |
|<a href="https://www.microsoft.com/en-gb/microsoft-365/onedrive/online-cloud-storage" target='_blank'>OneDrive</a>|&nbsp;&nbsp;  | Microsoft does offer OneDrive with a 5 GB free tier but space requirements for a system image may require further space for purchase at $19.99 p/a for 100 GB storage.|
|<a href="https://www.macrium.com/reflectfree?mo#" target='_blank'>Reflect8</a>|&nbsp;&nbsp;  | Macrium Reflect 8 billed as the best no-cost backup restore solution on the market.|
|<a href="https://www.easeus.com/backup-software/tb-free.html" target='_blank'>EaseUS</a>|&nbsp;&nbsp;  | No cost starter for full/differential/incremental backup and restore upgrade available at $19.95|
<a href="https://www.ubackup.com/free-backup-software.html" target='_blank'>AOMEI</a>|&nbsp;&nbsp;  | Free to download and use includes backup, recovery, clone, and sync functions.|
|<a href="https://www.paragon-software.com/free/br-free/" target='_blank'>PARAGON</a>|&nbsp;&nbsp;  | Free to download and use includes backup scheduling and selected recovery.|
|<a href="https://www.acronis.com/en-us/products/true-image/" target='_blank'>Acronis</a>|&nbsp;&nbsp;  | Subscription based backup, restore, malware protection in three flavours 'Essencial' @ $49.99 pa, 'Advanced' @ $89.99 pa, 'Premium' @ $124.99 pa.|


<u>**Mac Related**</u>

|Provider |&nbsp;&nbsp; | Comment|
|---------| ---  |  ---  |
|<a href="https://support.apple.com/en-us/HT204025"  target='_blank'>iDrive</a>|&nbsp;&nbsp; | iDrive offers 5TB for $79.50 at the time of writing 90% discount was available for the first year i you are using and alternative backup service ( Carbonite, Mozy, CrashPlan, Backblaze, SOS Online Backup, Dropbox and Google Backup and Sync.)|