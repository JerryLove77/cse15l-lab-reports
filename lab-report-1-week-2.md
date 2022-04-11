**This is Jianrui Zhang 's lab report**

> Installing VScode

Installing the best fitable version for you(Windows,Mac,Linux)

![Image](https://user-images.githubusercontent.com/103210019/162644154-05a0d1a3-48aa-4280-b3b3-6aab167a5c89.png)

> Remotely Connecting

type `ssh cs15lsp22zz@ieng6.ucsd.edu`. Replace `zz` by your course-specific account.

![Image](https://user-images.githubusercontent.com/103210019/162644182-52539f25-f47f-4312-996b-c44c14199f88.png)

> Trying Some Commands

`cd ~` :file system starts at home

`ls -lat` : brings up a list of hidden files

`pwd` : print working directory

![Image](https://user-images.githubusercontent.com/103210019/162669659-3f7e90a7-3cac-4bd8-bcc6-534e0816a30c.png)

> Moving Files over SSH with scp

The command is called `scp`.

![Image](https://user-images.githubusercontent.com/103210019/162644264-2ae7d3ea-7e55-44e7-8cd0-ff41b9a57262.png)

> Setting an SSH Key

type `ssh-keygen` 

![Image](https://user-images.githubusercontent.com/103210019/162668497-ce9be951-c5da-472a-a605-bd5ea91d10d0.png)

type `scp /Users/<user-name>/.ssh/id_rsa.pub cs15lsp22zz@ieng6.ucsd.edu:~/.ssh/authorized_keys`. 

then type your password! 

![Image](https://user-images.githubusercontent.com/103210019/162668573-9be320c4-caa4-470e-8fd2-2aa59dac1b54.png)

> Optimizing Remote Running

You can use semicolons to run multiple commands on the same line in most terminals.

![Image](https://user-images.githubusercontent.com/103210019/162670593-c001106c-b1ab-4003-8d9d-d7f184a29040.png)
