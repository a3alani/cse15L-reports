# Lab report 2


> https://github.com/a3alani/markdown-parser/blob/main/MarkdownParse.java

Notes) 
> The following screenshot includes the failure indcuing tests inputs followed by screenshots of the test file and terminal output

---
<img width="1440" alt="Screen Shot 2022-05-02 at 11 36 55 PM" src="https://user-images.githubusercontent.com/103146838/166413265-bfc1337d-9e18-42b1-987d-785bf36722c5.png">

---

1) First failure inducing test:

https://github.com/a3alani/markdown-parser/blob/main/test2.md

I added double brackets at the end of the link url
This caused MarkdownParse.java to go in an infinite loop when running. 

<img width="606" alt="Screen Shot 2022-05-02 at 7 32 45 PM" src="https://user-images.githubusercontent.com/103146838/166396829-09e7e149-270b-475e-93c3-567e0a337642.png">


<img width="543" alt="Screen Shot 2022-05-02 at 6 46 11 PM" src="https://user-images.githubusercontent.com/103146838/166395677-eba58db1-020e-4998-8f7f-05c5f8d17a9c.png">

---

2) Second failure inducing test:

https://github.com/a3alani/markdown-parser/blob/main/test3.md

I added curly brackets around the link url instead of parathesis. This caused MarkdownParse.java to throw an indexoutofbound exception.

<img width="602" alt="Screen Shot 2022-05-02 at 7 31 43 PM" src="https://user-images.githubusercontent.com/103146838/166396847-73db2bc8-2a66-4f72-a2cf-20ad2df56f38.png">


<img width="706" alt="Screen Shot 2022-05-02 at 7 06 08 PM" src="https://user-images.githubusercontent.com/103146838/166395467-768bec14-15db-4176-b54e-9dd9c3adabe9.png">

---

3) Third failure inducing test:

https://github.com/a3alani/markdown-parser/blob/main/test4.md

I did not add a parathesis before the link url and only after which caused the output of the wrong output.

<img width="726" alt="Screen Shot 2022-05-02 at 7 35 23 PM" src="https://user-images.githubusercontent.com/103146838/166396858-d3317b3f-99ae-4fe7-b762-8dd1a98ff77a.png">

<img width="662" alt="Screen Shot 2022-05-02 at 7 07 20 PM" src="https://user-images.githubusercontent.com/103146838/166395501-366b06c1-457e-464b-a1bc-ee0366bc0d16.png">

---

4) Another failure inducing test: (trying to cover other cases and replace incase any of my main 3 are not valid)

I added a new empty line after the link which caused the program to go into an infinite loop

<img width="706" alt="Screen Shot 2022-05-02 at 7 34 41 PM" src="https://user-images.githubusercontent.com/103146838/166396889-95807dab-3e5c-4886-85c0-28255cc61e3a.png">


<img width="677" alt="Screen Shot 2022-05-02 at 7 14 00 PM" src="https://user-images.githubusercontent.com/103146838/166395564-78ce9055-de34-4579-9ad2-9bb6b7a52bf2.png">

5)

I did not add a parenthesis at the end of the url link




<img width="682" alt="Screen Shot 2022-05-02 at 7 04 52 PM" src="https://user-images.githubusercontent.com/103146838/166395622-50c1590f-7efc-4ade-b45f-7a1361a3318b.png">

---

General Definition:

> A bug is a flaw in the computer system that may have zero or many symptoms. While a symptom is a faulty program behavior. As for the failure inducing input it causes the bug to excute and symptoms to appear.

* For the first test, the failure inducing input was adding the second parathesis at the end of the url link. That caused the bug to execute and the  symptom to appear as the program went into an infnite loop.

* For the second test, the failure inducing input of replacing the paraenthesis with curly brackets caused the program bug to execute because the parathesis was not detected as expected. That caused the symptom to appear and throw and indexOutOfBound exception in the terminal

* For the third test, the failure inducing input of not adding a parathesis before the url link did not cause a bug but instead resulted in a wrong output than expected

* For the fourth test, the failure inducing input of adding an empty line after the url caused a bug and resulted the program to go into an infinite loop.

* As for the last test, failure inducing input of not having a closing parenthesis also caused a bug that resulted in a symptom of an infinite loop.
