# Lab Report 4

1) A link to your markdown-parse repository and a link to the one you reviewed in week 7:

* Mine: https://github.com/a3alani/markdown-parser.git
* Reviewed: https://github.com/kcyy127/markdown-parser

---

2) For each test above:
- Decide on what it should produce (i.e., expected output) by using either VScode preview or the CommonMark demo site

Snippet 1)
* Expected:
["`google.com, "google.com", "ucsd.edu"]

---

Snippet 2) 
* Expected:
["a.com", "a.com(())", "example.com"]

---

Snippet 3)
* Expected
["https://www.twitter.com", "https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule", "https://cse.ucsd.edu/"]

---

- Showing the code in MarkdownParseTest.java for how you turned it into a test

<img width="610" alt="Screen Shot 2022-05-30 at 1 06 08 PM" src="https://user-images.githubusercontent.com/103146838/171054270-c751def6-0368-4d37-83b6-6ac71b15e333.png">


- For your implementation, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.


<img width="930" alt="Screen Shot 2022-05-30 at 1 15 32 PM" src="https://user-images.githubusercontent.com/103146838/171054961-f1c8358a-412d-4387-ae4c-cf23ab811b2f.png">

When I ran the program it went into an infinite loop. It did not pass

- For the implementation you reviewed in Week 7, the corresponding output when running the tests; if it passed, say so. If it didn’t pass, show the specific part of the JUnit output that shows the test failure.

<img width="1440" alt="Screen Shot 2022-05-30 at 1 19 12 PM" src="https://user-images.githubusercontent.com/103146838/171055326-628f2709-8cd5-4aa1-b243-d43608c2fe46.png">

The screenshot is showing an IO excpetion error, I do not know why this error is showing in the implementation I reviewd. However it is also expected not to pass the tests.


3) Answer the following questions with 2-3 sentences each:

- Do you think there is a small (<10 lines) code change that will make your program work for snippet 1 and all related cases that use inline code with backticks? If yes, describe the code change. If not, describe why it would be a more involved change.

Yes, the change would be to start from the index of the sqaure bracket which will skip over the backtick


- Do you think there is a small (<10 lines) code change that will make your program work for snippet 2 and all related cases that nest parentheses, brackets, and escaped brackets? If yes, describe the code change. If not, describe why it would be a more involved change.

I think the test will run and pass on the expected output, but in order to include other link in the nested link it will require a code change less than 10 lines. Like adding a condition that checks for nested links using matching open and closed parathenthesis and square brackets.


- Do you think there is a small (<10 lines) code change that will make your program work for snippet 3 and all related cases that have newlines in brackets and parentheses? If yes, describe the code change. If not, describe why it would be a more involved change.

I think the test will pass on the expected output which is whats highlighted in blue. However no, I do not think there will be a code chnage < 10 lines that will fix the program to include all links because there will be many conditions to consider like the spaces and separate lines between the links. 

