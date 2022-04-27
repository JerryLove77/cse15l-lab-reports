**This is Jianrui Zhang's Lab Report 2: Debugging and Testing**

Here are three changes:

# 1.Avoid images

![image](https://user-images.githubusercontent.com/103210019/165450731-bbd8cff4-1d4d-4aef-b298-7ec9b7be17e1.png)

> link to the test file: [test-file1](https://github.com/JerryLove77/markdown-parser/blob/main/TestFile1.md)

> Symptom of the input
![image](https://user-images.githubusercontent.com/103210019/165457645-7e95f600-26b4-4982-b206-bf2c1f69c708.png)


> The symptom of this error is caused by the markdown image and link formats being similar. By producing an image in the test file, the input causes this symptom.

> We avoid reporting picture file names in this case by inspecting the **!** symbol in the file. Specifically, its placement in relation to the sign **[**

# 2.Avoid checking previous indices(infinite loop)

> Link to the test file: [test-file1](https://github.com/JerryLove77/markdown-parser/blob/main/TestFile1.md)

> Symptom of the input
![image](https://user-images.githubusercontent.com/103210019/165458454-6cabd47a-ce92-422e-949e-e77728ff5319.png)


> The symptom of this bug is cause by the empty spaces at the end of document. The while loop will keep looking for letters because the index will never reach the finish because there is empty space at the end. By inserting a few blank spaces at the end of the file, the input causes the problem.**

> For this problem, we check if **closeBracket** is less than current index to ensure that the loop does not continue if previous repeated indices are being checked. As soon as the loop verifies **closeBracket** of previous indices, the loop will break.**

# 3.Checking correct link Markdown format

> link to the test file: [test-file3](https://github.com/JerryLove77/markdown-parser/blob/main/TestFile3.md)

> Symptom of the input
![image](https://user-images.githubusercontent.com/103210019/165458855-811e7eed-48b8-44a4-857f-5bd8fd4ba353.png)


> The symptom of this error is caused by printing the link even when the format is incorrect. When the spaces between **[]** and **()** are present in the form, the link will still be printed. With a gap between **]** and **(**, the input causes the bug.

> For this bug, we check if **closeBracket's** next index is **openParen**, which checks for spaces between the symbols.
