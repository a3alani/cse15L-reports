# Welcome to CSE 15L

My name is Ali and I will guide you on how to log in a course-specific account in this tutorial.

---

* __VS Code__

First step is to install VS Code. You can download VS Code through this link [VSCode](https://code.visualstudio.com/download).

<img width="1440" alt="Screen Shot 2022-03-31 at 6 23 56 PM" src="https://user-images.githubusercontent.com/103146838/162669390-e149f994-d434-4e0b-ba0f-8bf9c63324f8.png">

---

* __Remote Connecting__

Second you are going to connect to a remote system using SSH. If you are using a Windows you need to install [openSSH](https://docs.microsoft.com/en-us/windows-server/administration/openssh/openssh_install_firstuse). 

1) Look up your course-specifc account using this [Link](https://sdacs.ucsd.edu/~icc/index.php).

2) Open a terminal in VSCode and type the following command:
`ssh cs15lsp22zz@ieng6.ucsd.edu`

Note) <u>replace the "zz" with your course-specifc user.</u>

3) Enter yes when asked: 
> Are you sure you want to continue connecting (yes/no/[fingerprint])?

4) Enter your password and you should be logged in!

<img width="479" alt="Screen Shot 2022-03-31 at 6 50 13 PM" src="https://user-images.githubusercontent.com/103146838/162669773-cc039845-4d90-4922-b74f-60ca16d5e5e0.png">


---

* __Commands__

Next you are going to try running some commands.
Start by typing ls in your terminal, this should list all the files available. 

You can find more commands to test on Canvas Modules.

<img width="460" alt="Screen Shot 2022-03-31 at 6 28 48 PM" src="https://user-images.githubusercontent.com/103146838/162669848-782d6797-3f34-44e4-b522-11dc3adfcd40.png">

---

* __SCP__

Next your are going to move files with SCP. SCP allows you to copy file(s) from your computer to a remote computer.

1) In your terminal, type: 
`scp file.java cs15lsp22zz@ieng6.ucsd.edu:~/`

Note) <u> replace file.java with a file that you create, compile and run. </u>

2) Enter your password. (Same as the one you used for SSH)

3) Then log in into ieng with SSH again and type ls in your terminal. You should be able to see the file in your home directory

<img width="631" alt="Screen Shot 2022-03-31 at 6 54 52 PM" src="https://user-images.githubusercontent.com/103146838/162669932-cb0953a1-ccfe-4a0e-8e3c-d770a085cac4.png">

---

* __SSH Key__

Now you are going to set up SSH Key. This will allow you to login using keys instead of having to type your password everytime you login to ieng with SSH. 

1) On your computer, type ssh-keygen in the terminal 

2) Enter:
`/Users/user-name/.ssh/id_rsa`

 Note) *Change "user-name" with your own.*
 
 
 Tip) *Use the image as a reference*

3) Enter passphrase (empty for no passphrase)
    

4) Now if your try to login with ieng with SSH, you should be able to without entering your password!

<img width="500" alt="Screen Shot 2022-03-31 at 7 11 43 PM" src="https://user-images.githubusercontent.com/103146838/162669986-81feb478-909f-4739-b2f0-903224d7ed7e.png">

---

* __Remote Running__

Finally you are going to learn how to optimize remote running. 
1) You can write command in quotes at the end of SSH i.e) ssh cs15lsp22zz@ieng6.ucsd.edu "ls"

Note) This command will login in a list the home directory on the remote server directly

2) You can run multiple commands using semicolon ;

I.e) `cp WhereAmI.java OtherMain.java; javac OtherMain.java;`
 
<img width="510" alt="Screen Shot 2022-03-31 at 7 16 23 PM" src="https://user-images.githubusercontent.com/103146838/162670524-18e83874-eb6c-43aa-9281-21c659084f7e.png">

---

*Contragulations on completing the tutorial!*

 If you have any questions feel free to come to office hours or tutor hours for help.

Good Luck!

