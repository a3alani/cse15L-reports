# Lab Report 5

* I used: 

> $ bash script.sh > results.txt


* Then vimdiff on results.txt

---

Test 1: 

[194.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md)

<img width="782" alt="Screen Shot 2022-06-09 at 1 50 49 PM" src="https://user-images.githubusercontent.com/103146838/172942915-ef8da18d-77d5-4e34-b494-1d335dc7fd6e.png">

Expected from results.text:

> []

Actual:

> [url]

Solution:

My markdown implementation did not consider this a valid link but the given markdown file did display it as a link.

> <p><a href="my_(url)" title="title (with parens)">Foo*bar]</a></p>

url should not be displayed as a valid link

First,the program should look for the opening & closing "[" "]"
Next, check if the content inside the "(" ")" is a valid link


---

Test 2:

[201.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md)

<img width="764" alt="Screen Shot 2022-06-09 at 1 51 13 PM" src="https://user-images.githubusercontent.com/103146838/172942958-f444fc02-aa01-4cf0-a91b-b4867673366e.png">

Expected from results.txt:

> []

Actual:

> [baz]

Solution:

My markdown implementation considered this a valid link and the given markdown file did also display it as a link.

> <p>[foo]: <bar>(baz)</p>
> <p>[foo]</p>

baz should not be displayed as a valid link.

The program should not only check for "[" & "]" but also "](" so that the syntax is valid for a link.


---
---

Output for running main tests on both my implemenation and given markdownparser:

<img width="913" alt="Screen Shot 2022-06-06 at 11 44 50 PM" src="https://user-images.githubusercontent.com/103146838/172313748-27300668-fe30-4b49-aef8-1715ff0cca41.png">

<img width="1440" alt="Screen Shot 2022-06-06 at 11 46 17 PM" src="https://user-images.githubusercontent.com/103146838/172313955-93b3b919-3889-456d-82cc-b86d22b8ca32.png">

<img width="1440" alt="Screen Shot 2022-06-06 at 11 46 33 PM" src="https://user-images.githubusercontent.com/103146838/172313968-08403fce-0c69-4a4b-8d33-c5836669dc4e.png">

<img width="1440" alt="Screen Shot 2022-06-06 at 11 50 58 PM" src="https://user-images.githubusercontent.com/103146838/172314814-d95f6915-a8c9-49a3-8aad-ae53d58b13f7.png">
