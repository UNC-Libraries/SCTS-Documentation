# Overview

- [GIT Set-up Instructions](#git-setup-instructions)
  - [Finding Aids: Setting Up Your Development Space](#finding-aids-setting-up-your-development-space)
  - [Install Git for Windows](#install-git-for-windows)
- [GIT/Sourcetree Troubleshooting](#git/sourcetree-troubleshooting)
  - [Sourcetree: SSH Key Fail](#sourcetree-ssh-key-fail)
- [Oxygen Install and Transformation Scenario](#oxygen-install-and-transformation-scenario)
  - [Install Oxygen XML Editor](#install-oxygen-xml-editor)
  - [Set up Transformation Scenario](#set-up-transformation-scenario)

- [Merging and Pushing](#merging-and-pushing)

***

# GIT Set-up Instructions

## Finding Aids: Setting Up Your Development Space

### Overview

This how-to is intended for users who need to set up their computer to create and edit Finding Aid XML using Git and the Gitlab repository.  

### Assumptions/Requirements

This document assumes you're setting up your environment on a Windows machine and installing everything for the first time.  

## Install Git for Windows

1. Go to https://gitforwindows.org/ and download the installer (hit the "download" button and "Save File"  

2. Run the installer (probably saved to your Downloads folder), hitting "Next" and "Install" through all the prompts to do the default installation.  

3. When the installation is complete, uncheck "View Release Notes" and hit the "Finish" button.  

4. From the Start menu, go to Git and start Git GUI  

5. From the Git GUI window, click on Help > Show SSH Key  

6. If you already have an SSH key, it will show up here. If you don't, you should create a new one by hitting "Generate Key"  

7. The GUI will prompt you for a passphrase. You can leave this blank by hitting OK, and again on the following confirmation screen.  

8. Your SSH key will show up in the GUI window. Hit "Copy to Clipboard" and "Close"  

9. Go to the Start menu again and open Git > Git Bash. This will open a Linux-like command console  

10. Type "ssh gitlab.lib.unc.edu" and hit Enter.  

11. This will prompt you with a message about "authenticity of the host ... can't be established". Type "yes" and hit Enter.  

12. The console will prompt you for a password, but instead just type Ctrl + Z to exit the request.  

13. Now that you've established gitlab as a known host, you should be able to use Sourcetree to access Git. 


### Create an Account on GitLab and add an SSH Key

1. Go to your browser and load gitlab.lib.unc.edu.  

2. Log in with your onyen and password.  

3. If you don't already have access to the manuscripts/finding-aids repository, you'll need to have someone grant access. They can do that at https://
gitlab.lib.unc.edu/manuscripts/finding-aids/project_members.

4. Once you've logged into gitlab, go to "Profile Settings" in the left sidebar (or by clicking your profile icon in the top right) and click "SSH Keys" in 
the navigation along the top.  

5. Under 'Add an SSH Key", paste your public key text into the Key field and change the Title to something that identifies this computer ("Windows 
PC").

6. Hit "Add Key" to save the key to your profile.


### Install SourceTree

1. Download the installer from here: www.sourcetreeapp.com/download  

2. Save the file (to downloads or elsewhere) and run the exe.  

3. Sourcetree will prompt you to create a Bitbucket account (because they would like you to use their own Git tools, but we'll be using Github 
instead.)  
  a. If you already have an Atlassian or Bitbucket login, enter it now.  
  b. If not, create an account to activate the software, which will open their site in your browser.  
  c. After you create your account, it should take you to a page title "Confirm Access to Your Account". Click "Grant Access"  
  d. If Bitbucket doesn't open the Access page, go back to Sourcetree, hit the Back button, and press the Bitbucket link again to reopen their 
website.

4. Once you get the "Authentication Successful" message, go back to the Sourcetree app and you should see "Registration Complete!". Hit Next.

5. On the "Pick Tools" window, uncheck Mercurial and hit Next

6. On the "Preferences" window, make sure your name and email are correct (this is likely just for Atlassian's data collection) and hit Next.

7. You should see a popup titled "Load SSH Key?" Hit No.

8. You should next see a window titled "Remote Repositories". Ignore this and go to Tools > Options instead.

9. On the General tab, go to the SSH Client Configuration section and change SSH Client to "OpenSSH"

10. In the SSH Key field above, make sure it is pointing to your current SSH key location (probably C:\Users\your_username\.ssh\id_rsa)    

### Clone Repo from Gitlab in SourceTree

1. In SourceTree, go to the top left and click Clone/New and paste in the repo URL: git@gitlab.lib.unc.edu:manuscripts/finding-aids.git  

2. Set destination path to wherever you want to keep the files (it should default to Users\username\Documents\finding-aids)  

3. Sourcetree will take a moment to check the source of the repository. When it is done, click the Clone button.  

4. If it just quietly hangs, pretending to be checking the files, you should check to make sure that your machine is authenticating properly with the server by opening Putty and attempting to ssh to gitlab.lib.unc.edu.  

5. Assuming everything is working, Sourcetree should take just a moment to pull down all the files from the repository to your local repo.  


***

**References:**
- http://the.earth.li/~sgtatham/putty/0.58/htmldoc/Chapter9.html
- https://confluence.atlassian.com/sourcetreekb/generate-and-load-ssh-keys-into-sourcetree-with-putty-790629663.html
- https://confluence.atlassian.com/bitbucket/set-up-git-744723531.html

# GIT/Sourcetree Troubleshooting

## Sourcetree: SSH Key Fail

1. You have tried to pull or push to an existing branch in your Sourcetree repository and see the following notification:
 
![SSH_Key_Fail_Screen_1](https://user-images.githubusercontent.com/62359394/92785825-bc0e5300-f375-11ea-898c-d2d89bbd8f93.JPG "SSH Key Fail")

2. Click "no" and open the "Pageant PuTTY authentication agent" (computer wearing hat icon) by clicking on the "triangle" located on your Windows toolbar (bottom right corner), next to the wireless icon. You should see the the Pageant icon in this window.
 
![Pageant_1_Toolbar](https://user-images.githubusercontent.com/62359394/92786222-10b1ce00-f376-11ea-8e23-279e8bc93820.jpg "PuTTY authentication agent")

3. Click "Add Key" and navigate to the folder where GIT keeps your "finding-aids" folder (should be in "This PC>Documents"). Select "All Files" from drop-down to the right of "file name" field.You will want to select the "Microsoft Publisher" file that should be there named "id_rsa":

![SSH_RSA_Key ](https://user-images.githubusercontent.com/62359394/92786654-6c7c5700-f376-11ea-870a-5391745655f3.JPG "SSH RSA Key")


4. After clicking ok, the "Pageant Key List" should be populated and you can click "close." 

5. Try your pull/push request again.

# Oxygen Install and Transformation Scenario



## Install Oxygen XML Editor

1. Download the software at http://www.oxygenxml.com/xml_editor/software_archive_editor.html  

2. Choose version 23.  

3. Copy and paste information below into the license window (9 lines of text):

Registration_Name=Jackie Dean

Company=

Category=Academic

Component=XML-Editor, XSLT-Debugger, Saxon-SA

Version=23

Number_of_Licenses=8

Date=02-01-2021

Maintenance=0

SGN=MCwCFEf30fV8RourtRFEuBwgFMHqqXXJAhRY3L0F9IUSM/84znn302RyA4+bAA\=\=
   
## Set up Transformation Scenario

(Occasionally, you may have to recreate a new transformation scenario. Sometimes they just go away.) 

1. Open an EAD XML file in Oxygen. 

2. Click on the top horizontal menu's icon of a wrench with a red arrow 

3. In the pop-up box, select "New." 

4. Name your scenario something simple like "transformation_2021" 

_In the XSLT tab:_

5. XML URL should be: ${currentFileURL} (which it will be by default). 

6. XLS URL should point to our stylesheet: https://cdn.lib.unc.edu/faids/ead.xsl 

7. Select the transformer. Saxon EE 9.9.1.7. (or whatever the most up-to-date Saxon EE is) 

![Edit scenario screenshot 1](https://user-images.githubusercontent.com/58087302/79362917-2f21b380-7f15-11ea-8399-1f86a66559ea.png "Edit scenario window screenshot 1")

We don't use the FO Processor tab

_In the Output tab:_

8. In the Output File menu, the "Save as" box should be selected, and the value should be: ${cfn}.html 

9. If you would like for the resulting HTML file to automatically open in your Internet browser for preview, or in Oxygen for you to inspect, check the boxes for these options. 

10. Click "OK." You will be returned to the opening menu, but now you will see your new scenario appearing in the list of available transformation scenarios. 

> Note: If you forgot to name your scenario, it will automatically be named after the EAD XML file that you had opened when you began creating the scenario. To rename it, select it in the list and click "EDIT." Then change the name across the very top of the menu. Click "OK" to save your new scenario and return to Oxygen. 

![Edit scenario screenshot 2](https://user-images.githubusercontent.com/58087302/79363266-afe0af80-7f15-11ea-9754-3ce394c71b3c.png "Edit scenario window screenshot 2")



# Merging and Pushing

## Pushing New Finding Aid Changes Live

1. Make sure the correct branch is checked out on your local Sourcetree. If already under your local branches, pull any changes that need to be pulled. If the branch is not in your local branches, open your remote branches on the left hand side of Sourcetree, right click on the correct branch, and select "checkout origin/[branch]". A pop-up will ask you to confirm the checkout, click OK. 
![Remote branches](https://github.com/llsmith305/images/blob/main/Remote_branches.png?raw=true) 

*Remote branches*
<br>
<br>
![Branch checkout](https://github.com/llsmith305/images/blob/main/Branch_checkout.png?raw=true)
*Branch checkout*

2. Under your local branches, switch to the main branch by double-clicking on it.

3. While on the main branch, right click on the branch you want to go live and select "merge [branch] into current branch". In the pop-up, click OK to confirm the merge.
<br>

![Merge branch](https://github.com/llsmith305/images/blob/main/Merge_branch.png?raw=true)

*Merging the branch*
<br>
<br>
<br>
<br>
![Confirm merge](https://github.com/llsmith305/images/blob/main/Confirm_merge.png?raw=true)

*Confirm merging*

4. Push the new commits on main. In the Push pop-up, make sure the main branch is selected and click Push. The new changes to the main branch can take up to 2 hours to display live.

![Push main](https://github.com/llsmith305/images/blob/main/Push_main.png?raw=true)
*Pushing main branch*
