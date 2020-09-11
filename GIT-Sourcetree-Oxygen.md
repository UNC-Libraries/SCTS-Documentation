# Overview

- [GIT Set-up Instructions](#git-setup-instructions)
  - [Finding Aids: Setting Up Your Development Space](#finding-aids-setting-up-your-development-space)
  - [Install Git for Windows](#install-git-for-windows)
- [GIT/Sourcetree Troubleshooting](#git/sourcetree-troubleshooting)
  - [Sourcetree: SSH Key Fail](#sourcetree-ssh-key-fail)
- [Oxygen Install and Transformation Scenario](#oxygen-install-and-transformation-scenario)
  - [Install Oxygen XML Editor](#install-oxygen-xml-editor)
  - [Set up Transformation Scenario](#set-up-transformation-scenario)

***

# GIT Set-up Instructions

## Finding Aids: Setting Up Your Development Space

### Overview

This how-to is intended for users who need to set up their computer to create and edit Finding Aid XML using Git and the Gitlab repository.  

### Assumptions/Requirements

This document assumes you're setting up your environment on a Windows machine and installing everything for the first time.  

### Install Putty Tools

1. Google for putty tools. One good source is here: https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html 

2. Download the latest installer.exe (as of December 2017, it is putty-2017-07-08-installer.exe).  

3. Run the exe and install to your program files (the default X86/putty/ is fine).  

4. This should install Putty, Puttygen, and Pageant.  

### Run Puttygen to Generate SSH Keys

1. Go to Start > All Apps > Putty and run Puttygen.  

2. Select the "Key" tab and choose SSH2 RSA.  

3. Click Generate.  

4. Move your mouse randomly in the small screen in order to generate the key pairs.  

5. Leave your passphrase blank, or create one if you wish. It's not essential but it's more secure to use one. You will be asked for it when you connect via SSH.  

6. Click "Save private key" and save it as "id_rsa.ppk" in your documents folder (Users//My_Documents). You might put it there at the top or in an ssh or .ssh folder if you like. 

7. Click "Save public key" and save it as "id_rsa.pub" in the same place.  

8. Copy the public key text into a notepad screen, you'll need to paste it into Gitlab in a minute.  

9. Close Puttygen.  

### Add Keys to Pageant  

1. Check to see if Pageant is already running in your system tray on the bottom right; if not, go to the Start bar and start it.  

2. Click the Pageant icon with the right mouse button to open the menu and select ‘View Keys’  

3. When you first start Pageant, it has no keys, so the list box will be empty. To add a key to Pageant, press the ‘Add Key’ button.  

4. Navigate to your private key file (id_rsa.ppk) in this dialog and select it.  

5. Pageant will now load the private key. If the key is protected by a passphrase, Pageant will ask you to type the passphrase. When the key has been loaded, it will appear in the list in the Pageant window.  

6. If you want to remove Pageant from the System tray, click the right button on the Pageant icon, and select ‘Exit’ from the menu. Closing the Pageant main window does not shut down Pageant.  

### Install SourceTree [_THIS SECTION NEEDS UPDATING with latest version of Souretree AW_]

1. Download the installer from here: www.sourcetreeapp.com/download  

2. Save the file (to downloads or elsewhere) and run the exe.  

3. Create Atlassian account to activate the software.  

4. Skip bitbucket account. Window -> Load Key? say yes.  

5. In sourcetree, install embedded version of git.  

5. Mercurial window- "I don't want to use mercurial".  

7. The SourceTree interface should come up and be blank at this point.  

8. Go to Tools > Options > and use the SSH key field to browse to your Documents folder and set the location of your private key.  

### Create an Account on GitLab and add an SSH Key

1. Go to your browser and load gitlab.lib.unc.edu.  

2. Log in with your onyen and password.  

3. If you don't already have access to the manuscripts/finding-aids repository, you'll need to have someone grant access. mer 

4. In gitlab, go to "Profile Settings" in the sidebar and then "SSH Keys".  

5. Under 'Add an SSH Key", paste your public key text into the Key field and change the Title to something that identifies this computer ("Windows PC").  

### Clone Repo from Gitlab in SourceTree

1. Go to the top left and click Clone/New and paste in the repo URL: git@gitlab.lib.unc.edu:manuscripts/finding-aids.git  

2. Set destination path to wherever you want to keep the files (it should default to Users\username\Documents\finding-aids)  

3. Sourcetree will take a moment to check the source of the repository. When it is done, click the Clone button.  

4. If it just quietly hangs, pretending to be checking the files, you should check to make sure that your machine is authenticating properly with the server by opening Putty and attempting to ssh to gitlab.lib.unc.edu.  

5. Assuming everything is working, Sourcetree should take just a moment to pull down all the files from the repository to your local repo.  


If Putty doesn't work for you, follow these instructions:

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

2. Choose version 15.2.  

3. Copy and paste information below into the license window:  

   Registration_Name=Gregory Neville  

   Company=University of North Carolina at Chapel Hill  

   Category=Academic-Site  

   Component=XML-Editor, XSLT-Debugger, Saxon-SA Version=15  

   Number_of_Licenses=1 Date=06-13-2013  

   Maintenance=374 SGN=MCwCFFnvMwFb46l7evGVjmLvrQHbLdc+AhR4SOcVT5QvkKKRj1EdgHZDzj/+mA\=\=      
   
## Set up Transformation Scenario

(Occasionally, you may have to recreate a new transformation scenario. Sometimes they just go away.) 

1. Open an EAD XML file in Oxygen. 

2. Click on the top horizontal menu's icon of a wrench with a red arrow 

3. In the pop-up box, select "New." 

4. Name your scenario something simple like "transformation_2018" 

_In the XSLT tab:_

5. XML URL should be "${currentFileURL}" (which it will be by default). 

6. XLS URL should point to our stylesheet: http://cdn.lib.unc.edu/faids/ead.xsl 

7. Select the transformer. Saxon EE 9.5.1.3. 

![Edit scenario screenshot 1](https://user-images.githubusercontent.com/58087302/79362917-2f21b380-7f15-11ea-8399-1f86a66559ea.png "Edit scenario window screenshot 1")

We don't use the FO Processor tab

_In the Output tab:_

8. In the Output File menu, the "Save as" box should be selected, and the value should be: "${cfn}.html" 

9. If you would like for the resulting HTML file to automatically open in your Internet browser for preview, or in Oxygen for you to inspect, check the boxes for these options. 

10. Click "OK." You will be returned to the opening menu, but now you will see your new scenario appearing in the list of available transformation scenarios. 

> Note: If you forgot to name your scenario, it will automatically be named after the EAD XML file that you had opened when you began creating the scenario. To rename it, select it in the list and click "EDIT." Then change the name across the very top of the menu. Click "OK" to save your new scenario and return to Oxygen. 

![Edit scenario screenshot 2](https://user-images.githubusercontent.com/58087302/79363266-afe0af80-7f15-11ea-9754-3ce394c71b3c.png "Edit scenario window screenshot 2")
