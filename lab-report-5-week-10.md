# Lab Report 5

* I used: 

> $ bash script.sh > results.txt


* Them vimdiff on results.txt

---

Test 1: 

[194.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/194.md)

<img width="782" alt="Screen Shot 2022-06-09 at 1 50 49 PM" src="https://user-images.githubusercontent.com/103146838/172942915-ef8da18d-77d5-4e34-b494-1d335dc7fd6e.png">

Expected from results.text:

> []

Actual:

> [url]

Solution:



---

Test 2:

[201.md](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/201.md)

<img width="764" alt="Screen Shot 2022-06-09 at 1 51 13 PM" src="https://user-images.githubusercontent.com/103146838/172942958-f444fc02-aa01-4cf0-a91b-b4867673366e.png">

Expected from results.txt:

> []

Actual:

> [baz]

Solution:


* In the implementation, I reviewed the expected output was different than the actual
* The preview also presents a different output than expected

<img width="913" alt="Screen Shot 2022-06-06 at 11 44 50 PM" src="https://user-images.githubusercontent.com/103146838/172313748-27300668-fe30-4b49-aef8-1715ff0cca41.png">

<img width="1440" alt="Screen Shot 2022-06-06 at 11 46 17 PM" src="https://user-images.githubusercontent.com/103146838/172313955-93b3b919-3889-456d-82cc-b86d22b8ca32.png">

<img width="1440" alt="Screen Shot 2022-06-06 at 11 46 33 PM" src="https://user-images.githubusercontent.com/103146838/172313968-08403fce-0c69-4a4b-8d33-c5836669dc4e.png">


* For my MarkdownParse implementation:
* 1 passed while the other failed

<img width="1440" alt="Screen Shot 2022-06-06 at 11 50 58 PM" src="https://user-images.githubusercontent.com/103146838/172314814-d95f6915-a8c9-49a3-8aad-ae53d58b13f7.png">
