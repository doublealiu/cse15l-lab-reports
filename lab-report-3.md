# Lab Report 3

## Streamling SSH Config

Here is my ssh config, inside its directory and opened. I use just use NotePad++ to edit it:

![Image](/report-3-res/ssh_config_dir.png)

![Image](/report-3-res/ssh_config_notepad.png)

Here is me connecting to my remote server using this alias:

![Image](/report-3-res/ssh_connect_alias.png)

And here is me SCP-ing a file into my lab account:

![Image](/report-3-res/scp_alias.png)

## Setup Github Access from ieng6

Here is my public key on GitHub. It's named cse15l ieng6:

![Image](/report-3-res/ssh_keys_github.png)

And here it is on my lab account. This is also where my private key is stored:

![Image](/report-3-res/ssh_keys_user_account.png)

Here is me cloning my markdown-parser repository, deleting a file, committing, and then pushing the changes from my lab account:

![Image](/report-3-res/user_account_commit1.png)

![Image](/report-3-res/user_account_commit2.png)

And here is the link to the commit: [Click Me!](https://github.com/doublealiu/markdown-parser/commit/f4e0216d382103b7de00f4ea707709e427744fa9)

## Copy Whole directories with scp -r

Here is me cloning the repository on my computer, SCP-ing it into my lab account, and then manually logging in and compiling/running all the tests:

![Image](/report-3-res/part_3_1.png)

![Image](/report-3-res/part_3_2.png)

![Image](/report-3-res/part_3_3.png)

![Image](/report-3-res/part_3_4.png)

The test fails because I deleted a file in my commit for the lab report. Here is me doing all that in one scp command. I've already cloned the repository so I'm just running the SCP command:

![Image](/report-3-res/part_3_21.png)

![Image](/report-3-res/part_3_22.png)

For some reason the tests don't compile when I run them through this multiline command, but they run fine when I manually SSH in and run them.