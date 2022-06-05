# **Jianrui Zhang's Lab Report 5**

## Different Test:

For demonstration purposes, I would use `342.md` and`14.md` as two examples of different output from `my-markdown-parser` and the recent implement of `markdown-parser`.

I was able to find the tests with different results using `vimdiff` on the result.

Here is the links to the test files:

[Test 342](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/342.md)

[Test 14](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/14.md)

## Test 342

- For Test 342, my implements gave the correct output, which should be zero.

![Test 342](Test342-2.jpg)


![Test 342](Test342-1.jpg)

- On left side, my implement returns null; however, given implement returns a link

- The main fix for test 342 is regarding backticks in markdown. Backtick detection is required when running through the "link" because of the particular functions of backticks.

- As this is a small fix, backtick detection in the getLinks method or a new method is required.

![Test 342](Test342-3.jpg)

## Test 14

- For Test 14, my implements gave the correct output, which should be zero.

![Test 14](Test14-2.jpg)

![Test 14](Test14-1.jpg)

- On left side, my implement returns null; however, given implement returns a link

- The main fix for test 14 is regarding opening bracket in markdown.
Opening bracket detection is required after finding all deliminators that check whether there is a escape key ("`\`") preceding each deliminator. 

![Test 510](Test14-3.jpg)