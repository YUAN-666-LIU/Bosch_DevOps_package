# How to setup your Git

This tutorial will guide you how to set up git and connect to Bosch GitHub. If you don't know what is Git, please read this page [https://inside-docupedia.bosch.com/confluence/x/Dx-aeQ](https://inside-docupedia.bosch.com/confluence/x/Dx-aeQ)

## Download Git from IT Service Portal
step 1: apply Git
click "IS" on Bosch website
![图片](img\image2021-12-6_15-39-56.png)
Then click as pictures shown.
![图片](img\image2021-12-6_15-48-36.png)
Recommend  choose Source Tree + Git For Windows (install)
![图片](img\image2021-12-6_15-57-33.png)

## Setup git on PC
### Step 1: Check your git installation
After Git was applied on IT Service Portal, you will see the Git Bash in the program menu.
![图片](img\image2021-12-7_10-44-18.png)
### Step 2: Generate SSH key
Click Git Bash

input               git config --global user.name "Your GitHub User Name"
                       git config --global user.email "Your GitHub Email"
as below:
![图片](img\1321829-20180923143956552-688336164.png)
Then enter        ssh-keygen -t rsa -C "Your GitHub Email"

Press 3 times Enter key

We don't needs to set any password, until you can see this 
![图片](img\1321829-20180923144013122-745856687.png)

### Step 3: upload SSH Public key
.ssh File is usually under C:\Users\your NT
![图片](img\image2021-12-7_11-27-58.png)

copy all text in id_rsa.pub.

Past it in Settings > SSH and GPG keys > New SSH key
![图片](img\image2021-12-7_11-29-48.png)
![图片](img\image2021-12-7_11-32-2.png)

After paste the ssh key, click add SSH key

![图片](img\image2021-12-7_13-39-34.png)

## Setup VSCode
( If you use Source Tree. please skip this chapter)

### Step 1:
Clone a repository from GitHub in vs-code. It will pop out a window which asking for Token
![图片](img\2021-12-06_15h05_21.png)
### Step 2:  Get Token
Go to GitHub Settings > Developer settings > Personal access tokens. Click Generate new token.
![图片](img\image2021-12-7_14-59-55.png)
![图片](img\image2021-12-7_15-21-7.png)
You will get a line of text called token. Paste the token into Vscode
![图片](img\2021-12-06_15h05_21 (1).png)

Now you can clone, push and pull content from GitHub.

After carefully follow previous steps, click the red box to add change into Stage.
![图片](img\image2021-12-8_9-44-31.png)


When your selected file was added into Stage, you can commit it by click the check icon. Afterward, synchronize the change with the cloud base repository.
![图片](img\image2021-12-8_9-53-24.png)