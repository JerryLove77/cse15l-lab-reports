**This is Jianrui Zhang's Lab Report 2: Debugging and Testing**

Here are three changes:

# 1.Avoid images

![image](https://user-images.githubusercontent.com/103210019/165450731-bbd8cff4-1d4d-4aef-b298-7ec9b7be17e1.png)

> link to the test file: [test-file 1](https://github.com/JerryLove77/lab3/blob/main/test-file1.md)

> Symptom of the input

> The symptom of this error is caused by the markdown image and link formats being similar. By producing an image in the test file, the input causes this symptom.

> We avoid reporting picture file names in this case by inspecting the **!** symbol in the file. Specifically, its placement in relation to the sign **[**

# 2.Avoid checking previous indices(infinite loop)

> Link to the test file:

> Symptom of the input

> The symptom of this bug is cause by the empty spaces at the end of document. The while loop will keep looking for letters because the index will never reach the finish because there is empty space at the end. By inserting a few blank spaces at the end of the file, the input causes the problem.**

> For this problem, we check if **closeBracket** is less than current index to ensure that the loop does not continue if previous repeated indices are being checked. As soon as the loop verifies **closeBracket** of previous indices, the loop will break.**

# 3.Checking correct link Markdown format

> link to the test file:

> Symptom of the input

> The symptom of this error is caused by printing the link even when the format is incorrect. When the spaces between **[]** and **()** are present in the form, the link will still be printed. With a gap between **]** and **(**, the input causes the bug.

> For this bug, we check if **closeBracket's** next index is **openParen**, which checks for spaces between the symbols.
