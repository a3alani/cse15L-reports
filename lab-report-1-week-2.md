# Welcome to CSE 15L

My name is Ali and I will guide you on how to log in a course-specific account in this tutorial.

---

* __VS Code__

First step is to install VS Code. You can download VS Code through this link [VSCode](https://code.visualstudio.com/download).
![Image]()

---

* __Remote Connecting__

Second you are going to connect to a remote system using SSH. If you are using a Windows you need to install [openSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse). 

1) Look up your course-specifc account using this [Link](https://sdacs.ucsd.edu/~icc/index.php).

2) Open a terminal in VSCode and type the following command:
> ssh cs15lsp22zz@ieng6.ucsd.edu 

Note) <u>replace the "zz" with your course-specifc user.</u>

3) Enter yes when asked: 
> Are you sure you want to continue connecting (yes/no/[fingerprint])?

4) Enter your password and you should be logged in!

![Image]()

---

* __Commands__

Next you are going to try running some commands.
Start by typing ls in your terminal, this should list all the files available. 

You can find more commands to test on Canvas Modules.

![Image]()

---

* __SCP__

Next your are going to move files with SCP. SCP allows you to copy file(s) from your computer to a remote computer.

1) In your terminal, type: 
> scp file.java cs15lsp22zz@ieng6.ucsd.edu:~/

Note) <u> replace file.java with a file that you create, compile and run. </u>

2) Enter your password. (Same as the one you used for SSH)

3) Then log in into ieng with SSH again and type ls in your terminal. You should be able to see the file in your home directory

![Image]()

---

* __SSH Key__

Now you are going to set up SSH Key. This will allow you to login using keys instead of having to type your password everytime you login to ieng with SSH. 

1) On your computer, type ssh-keygen in the terminal 

2) Enter file in which to save the key
(/Users/<user-name>/.ssh/id_rsa): /Users/<user-name>/.ssh/id_rsa

Note) chnage <user-name> with your own

3) Enter passphrase (empty for no passphrase):

![Image]()

4) Now if your try to login with ieng with SSH, you should be able to without entering your password!

---

* __Remote Running__

Finally you are going to learn how to optimize remote running. 
1) You can write command in quotes at the end of SSH i.e) ssh cs15lsp22zz@ieng6.ucsd.edu "ls"

Note) This command will login in a list the home directory on the remote server directly

2) You can run multiple commands using semicolon ;

I.e) cp WhereAmI.java OtherMain.java; javac OtherMain.java;

---

*Contragulations on completing the tutorial!*

 If you have any questions feel free to come to office hours or tutor hours for help.

Good Luck!

