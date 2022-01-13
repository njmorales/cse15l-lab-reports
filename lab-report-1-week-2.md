Back to [All Labs](https://njmorales.github.io/cse15l-lab-reports/)
# Lab Report 1 - Logging onto ieng6 Tutorial

## Step 1: Installing VSCode
* Download Visual Studio Code [Here](https://code.visualstudio.com/)!
* After it has installed, open the program. It should look something like this:
![Image](vscodescreenshot.png)

## Step 2: Remotely Connecting
* If you are on Windows, you must first install a program called OpenSSH. You can do that by following this guide [Here](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse)!
* Lookup your course-specific account for CSE 15L [Here](https://sdacs.ucsd.edu/~icc/index.php)
* Your account name should resemble something like this (with the 'xx' portion replaced by your specific characters): 
>`cs15lwi22xx@ieng6.ucsd.edu`
* In VSCode, open the terminal and type this command: 
>`$ ssh cs15lwi22xx@ieng6.ucsd.edu`
* Type 'yes' if you recieve a message along the lines of this: 
>`The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])?`

* The terminal will then ask for your account password, so type that in and hit enter. You should then see something like this in your terminal:
![Image](sshlogin.png)

## Step 3: Trying Some Commands

## Step 4: Moving Files with scp

## Step 5: Setting an SSH Key

## Step 6: Optimizing Remote Running