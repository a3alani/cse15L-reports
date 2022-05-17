# Lab Report 3

1) __Streamlining ssh Configuration__

* Show your .ssh/config file, and how you edited it (with VScode,
another program, etc)

<img width="470" alt="Screen Shot 2022-05-09 at 12 31 22 PM" src="https://user-images.githubusercontent.com/103146838/167484007-638c03d9-6128-4773-a5d0-470343ae1c79.png">


* Show the ssh command logging you into your account using just
the alias you chose.

<img width="489" alt="Screen Shot 2022-05-09 at 12 31 54 PM" src="https://user-images.githubusercontent.com/103146838/167484018-02b3736a-5a7c-4fd6-adb3-0984f6881a9c.png">

* Show an scp command copying a file to your account using just the
alias you chose.

<img width="472" alt="Screen Shot 2022-05-09 at 1 10 16 PM" src="https://user-images.githubusercontent.com/103146838/167489547-44e288f4-8633-413f-9643-47b0e2a2ccb1.png">

<img width="880" alt="Screen Shot 2022-05-16 at 6 58 11 PM" src="https://user-images.githubusercontent.com/103146838/168712915-10f45918-9b64-420f-8991-30b79eb46930.png">

---

2) __Setup Github Access from ieng6__

* Show where the public key you made is stored on Github and in
your user account (screenshot).

<img width="1440" alt="Screen Shot 2022-05-09 at 12 51 51 PM" src="https://user-images.githubusercontent.com/103146838/167489649-5b6d1493-5a67-4934-8561-ea2e438b8840.png">

* Show where the private key you made is stored on your user
account (but not its contents) as a screenshot.

<img width="805" alt="Screen Shot 2022-05-09 at 1 16 19 PM" src="https://user-images.githubusercontent.com/103146838/167490433-02c41225-3e43-46c1-8371-678b3dd550cd.png">

* Setting up Github access from ieng6:

1) Clone MarkdownParse repository through pasting git clone (HTTPS link) in the terminal
2) Change directory to MarkdownParse repository
3) In the terminal, paste git remote set-url origin (repo SSH url)
4) Enter touch test.txt
5) Enter git add .
6) Enter git commit -m "new change"
7) Then git push

* Show running git commands to commit and push a change to
Github while logged into your ieng6 account.

<img width="632" alt="Screen Shot 2022-05-16 at 7 30 14 PM" src="https://user-images.githubusercontent.com/103146838/168716283-ee5b2128-ab8e-4d8f-8c6e-535fcb2c4de5.png">

* Show a link for the resulting commit.

https://github.com/a3alani/markdown-parser/commit/d00a6083bfc06087c58cdf4bfde56e870d721568

---

3) __Copy whole directories with scp -r__

* Enter `scp -r . cs15lsp22asv@ieng6.ucsd.edu:~/markdown-parse` in the terminal to copy the whole direcotry into the server 

Show copying your whole markdown-parse directory to your ieng6
account.

<img width="1125" alt="Screen Shot 2022-05-16 at 7 55 54 PM" src="https://user-images.githubusercontent.com/103146838/168720494-31c83c20-3c7f-4054-b266-1a3756adc259.png">

<img width="905" alt="Screen Shot 2022-05-16 at 8 02 18 PM" src="https://user-images.githubusercontent.com/103146838/168720504-1a19a73b-bc16-47c5-962c-07e42b68742f.png">


Show logging into your ieng6 account after doing this and compiling
and running the tests for your repository.

<img width="905" alt="Screen Shot 2022-05-16 at 8 02 18 PM" src="https://user-images.githubusercontent.com/103146838/168721449-a36a3741-d28c-45c1-b9ba-c53d759ee88d.png">

<img width="1116" alt="Screen Shot 2022-05-16 at 8 14 41 PM" src="https://user-images.githubusercontent.com/103146838/168721455-6d3d6465-42fb-41b6-b1a9-a71736a79da3.png">



Show (like in the last step of the first lab) combining scp, ;, and
ssh to copy the whole directory and run the tests in one line.

* remove directory and then copy again using semi-colon for multiple commands in one line
