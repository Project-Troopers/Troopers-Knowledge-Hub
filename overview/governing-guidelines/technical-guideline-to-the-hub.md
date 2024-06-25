---
description: This is a short overview on the technical structure of the hub.
---
# Technical Guideline to the Hub

The Hub and the Project depends on a series of software technologies, handshakes and built-in models. This section is present under the purview of the Legal Stature of the hub.

## GitBook

GitBook is the documentation software on which the hub is located. This page, the website, the sub-domain of hosting, well, most of the software is provided by GitBook. View the required GitBook documentation in the official site linked below, to learn about the editing features.

{% embed url="https://docs.gitbook.com/" %}
The Documentation
{% endembed %}

### GitHub

Since we can't add all the members of the project on GitBook due to technical limitations, we have used GitSync (by GitBook) to sync our documentation with GitHub. It is available at the link listed below. Only members with authorized access roles are allowed to commit to it.

{% embed url="https://github.com/Project-Troopers/Troopers-Knowledge-Hub/tree/main/Knowledge%20Hub" %}
Our Files on GitHub
{% endembed %}

### Google Drive

We used to, and still continue to, hold an archive of all the materials that we link in this documentation on Google Drive. We may not include URLs, however.

The link to the back end is[ Jugzards - CBSE](https://drive.google.com/drive/folders/1H6GLo8tvjuDqWGfHuYQiZo\_WkKoVZmJX?usp=drive\_link).

## Offline Access to the Hub
The Hub can be completely accessed offline, using Git and Obsidian.

{% hint style="info" %}
#### **Recommended Specs to use the Hub offline**
1. **Space**: 15 GB Recommended, 5 GB Minimum
2. **Network**: 50 Mbps speed recommended, 10 Mbps speed minimum
{% endhint %}

{% hint style="danger" %}
#### **Minimum Specs to use the Hub offline**
1. **Space**: 5 GB
2. **Network**: 
{% endhint %}
### For Windows Users
1. You'll need Git and Obsidian software. To download the required applications, use the following command.
```
winget install Git.Git Obsidian.Obsidian
```
2. Then, you'll need to clone the hub locally so that it'll work on device. To do that, type the following commands. 
```
cd Documents
git clone https://github.com/Project-Troopers/Troopers-Knowledge-Hub.git --progress
```
*Footnotes: cd Documents will select the Documents folder on device (not on any online service) locally, and you change it to any directory.*
3. After cloning it on device, open Obsidian. Then click on open a new vault. 
4. In the address bar of File Explorer, paste this directory, and then click on "Open" (or "select folder".)
```
%USERPROFILE%\Documents\troopers-knowledge-hub\
```
5. 