# Lab Report 4

1) A link to your markdown-parse repository and a link to the one you reviewed in week 7:

* Mine: https://github.com/a3alani/markdown-parser.git
* Reviewed: https://github.com/kcyy127/markdown-parser

---

2) For each test above:
- Decide on what it should produce (i.e., expected output) by using either VScode preview or the CommonMark demo site
* Expected:

Snippet 1)
* [a link](url.com)
* another link` `
* cod[e
* code]

---

Snippet 2) 
* [a nested link](b.com)
* a nested parenthesized url
* some escaped [ brackets ]

---

Snippet 3)
* [this title text is really long and takes up more than one line
* and has some line breaks]( https://www.twitter.com )
* this title text is really long and takes up more than one line
* [this link doesn't have a closing parenthesis](github.com
* And there's still some more text after that.
* [this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/
* )
* And then there's more text

---

- Showing the code in MarkdownParseTest.java for how you turned it into a test

<img width="476" alt="Screen Shot 2022-05-23 at 1 57 53 PM" src="https://user-images.githubusercontent.com/103146838/169905751-c7b80447-942a-40e0-bebf-24521227bde5.png">

<img width="450" alt="Screen Shot 2022-05-23 at 2 02 19 PM" src="https://user-images.githubusercontent.com/103146838/169905756-f8418f3d-3538-4306-86e8-a9cb2a9758de.png">


- For your implementation, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.


- For the implementation you reviewed in Week 7, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.

3) Answer the following questions with 2-3 sentences each:

- Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

Yes, the change would be to start from the index of the sqaure bracket which will skip over the backtick


- Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.

No, I do not think there will be a code chnage < 10 lines that will fix the program. It will require a more involved chnage


- Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.

No, I do not think there will be a code chnage < 10 lines that will fix the program. It will require a more involved chnage


- If your code already works on some/all test cases, include an explanation of what were the code changes that allowed the tests to pass.



4) If you’re using a direct clone to ieng6, you might find it useful to give an extra argument to git clone that specifies which directory to clone into, for example:
$ git clone https://github.com/ucsd-cse15l-sp22/markdown-parse markdown-parse-target-directory
