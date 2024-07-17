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

{% @github-files/github-code-block url="https://github.com/Project-Troopers/Troopers-Knowledge-Hub/" %}

### Google Drive

We used to, and still continue to, hold an archive of all the materials that we link in this documentation on Google Drive. We may not include URLs, however.

The link to the back end is[ Jugzards - CBSE](https://drive.google.com/drive/folders/1H6GLo8tvjuDqWGfHuYQiZo\_WkKoVZmJX?usp=drive\_link).

## Offline Access to the Hub

The Hub can be completely accessed offline, using Git and Obsidian.

{% hint style="info" %}
**Recommended Specs to use the Hub offline**

1. **Space**: 15 GB Recommended, 5 GB Minimum
2. **Network**: 50 Mbps speed recommended, 10 Mbps speed minimum
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

_Footnotes: cd Documents will select the Documents folder on device (not on any online service) locally, and you can change it to any directory._&#x20;

3. After cloning it on device, open Obsidian. Then click on open a new vault.&#x20;
4. In the address bar of File Explorer, paste this directory, and then click on "Open" (or "select folder".)

```
%USERPROFILE%\Documents\troopers-knowledge-hub\
```

5. Then click on "Trust". After that, go to the settings icon near the name of the workspace, click on community plugins, enable the community plugins part.
6. Enable the Git Plugin. Go to the Settings (Gear Icon) of the Git Plugin and set Hostname to any name to identify your device with.

That's all. Sync has been set up!

* If you have access to edit the repository then you can automatically edit it from there itself.
* If you don't, just don't edit the text files, as it will force an commit update which you might not have permission to do so. In order to prevent accidental edits from happening, you can turn on the "Reading View" by clicking on the book icon near top-right corner of the app.

## For Android/iOS/iPadOS users

{% hint style="info" %}
**Prerequisite Steps**

1. Download the Obsidian app from your respective app store.
2. Create a dummy vault in the Obsidian app, to expose the Obsidian folder to the operating system. Close the app.
3. For the next steps alone, you will need to create a GitHub account with a "Classic Personal Access Token". First, create a GitHub account.
4. Then go to this link: [Personal Access Tokens (Classic) · GitHub](https://github.com/settings/tokens) and create a Personal Access Token with the "repo" option ticked (it will automatically tick all the sub-options under it). **Copy the token and store it safely, you will need it later.**
5. Then download this snapshot of the hub that is stored on our drive. -> [Troopers-Knowledge-Hub.zip - Google Drive - Snapshot](https://drive.google.com/uc?export=download\&id=1ZHLTrpX3hhfaVD6O45d4IWghg5YfhdVD)
{% endhint %}

1. Now extract the zip file and place the extracted folder in the Obsidian app folder located on your device.
   * **Android**: Internal Memory -> Obsidian (which is `/storage/emulated/0/Obsidian`)
   * **iOS**: On my iPhone or On my iPad -> Obsidian folder (with the obsidian logo.)
2. Now turn off Wi-Fi and mobile data, and open Obsidian.
3. Switch to the vault with the name "Troopers-Knowledge-Hub".
4. Open the Command palette (if you're on mobile, this will located in the 3-lines menu option in the bottom bar. The icon of the "Command palette" in the sub-menu will be a command prompt/terminal).
5. Run the command and click on **yes** when prompted. (**DON'T SKIP THIS STEP.**)

```
git: CAUTION: Discard all changes
```

6. Open Obsidian, click on the Gear icon in the menu that is on the left (if on mobile, pull from the left side to view it).
7. Go to _Community Plugins -> Git Settings_ (click on the gear icon next to the git plugin)
8. Scroll down to the author information section and fill out the Username (GitHub) and Personal Access Token box.
9. Close the dialog box and repeat steps 11 and 12. Now scroll down to author information again and fill out the author name and email with your details.
10. Turn back Wi-Fi/Mobile Data On, and open the Command palette (if you're on mobile, this will located in the ==3-lines menu option== in the bottom bar. The icon of the "**Command palette**" in the sub-menu will be a command prompt/terminal).
11. Type in the command.

```
git: pull
```

12. Wait for the app to show a pop-up notification near the bottom that states "Finished pull".

{% hint style="success" %}
**Now, your vault is ready! You can view the hub offline whenever you want. Few pointers**:

* If you have access to edit the repository then you can automatically edit it from there itself.
* If you don't, just don't edit the text files, as it will force an commit update which you might not have permission to do so. In order to prevent accidental edits from happening, you can turn on the "Reading View" by clicking on the book icon near top-right corner of the app.
{% endhint %}
