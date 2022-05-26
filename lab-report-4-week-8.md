# This is Jianrui Zhang's Lab Report 4 

## MarkdownParse Snippet tests:

 Repo used

- [My Repo](https://github.com/JerryLove77/markdown-parser)

- [Reviewed Repo](https://github.com/yuxinguo13/markdown-parser)

Tests in `MarkdownParseTest.java`:

- Variables used:
![variable](variableused.png)

- Test for my `MarkdownParse.java`:
![Test](MyTest.png)

- Test for reviewed `MarkdownParse.java`
![Review](ReviewTest.png)


## Results for my implementation:

- non of three tests passed

- All of the errors are assertion errors 

-  my implementation failed to capture the proper link for each test.

![Result](MyResult.png)

## Results for reviewed implementation:

- non of three tests passed

- There is a memory and an out of bounds exception, both of which need to be fixed in the implementation.

![ReviewResult](ReviewResult.png)

## Solution to the tests

### Fixes for snippet 1:

- There should be a small fix for the inline code with backticks senario

- The demo of the fix 
![fix](fix1.png)

### Fixes for snippet 2:

- There would be a major fix on the original code

- detect open and close parenthesis and brackets need to be revised

### Fixes for snippet 3:

- There should be a small fix on the original code for cases in snippet 3.

- fix the issue about the blank spaces and newlines
