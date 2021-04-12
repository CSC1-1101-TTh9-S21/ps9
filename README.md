# Problem Set 9

### Due Tuesday, April 20, 2021, at 11:59pm EST

As always, you will submit to Canvas **a single .zip file**. Detailed instructions for what the .zip file should contain are at the end of this problem set. 

Download this whole directory to your desktop, unzip it, and carry out the tasks described below.


---

## Part 1: Revisiting Problem Set 7
For this part of the problem set, find `ps7-buggy.py` in the `ps7` folder within this folder. I took my solution for ps7, and I introduced an bug in each of the 5 image functions (`colorswitch()`, `fliphorizontal()`, `greyscale()`, `monochrome()`, `upsidedown()`). Your goal will be to test the program in order to identify these 5 bugs. 

In 4 of the 5 functions, the bug causes the whole program to crash. You will have to look at the stack trace and the code to identify and repair the bug.

In the remaining function, the bug will not cause the program to crash. Instead, it will edit the image in an unintended way.

Here is what you need to do:

1. Create a document using a text editor, Word, Google Docs, latex, or your preferred document creation software.

2. In the document, for each of the 5 functions (`colorswitch()`, `fliphorizontal()`, `greyscale()`, `monochrome()`, `upsidedown()`), provide the following information:

* Reproduce the error from the stac trace (if it's one of the bugs that crashes the program) or describe the problem (if it's the bug that just has an unintended effect on the image).
* Reproduce the line of code that triggered the error (i.e., the one in the stack trace or the one that messes up the output).
* If there is a line earlier in the code that is actually causing the problem, also reproduce that line.
* Describe a few sentences what the bug is and how someone might have made that mistake.
* Describe how you would fix the error. 

3. In the code of the program, fix the error.

For instance, if you were given this code

```
a = 5
b = "tree"
c = a + b
```

I'd want to see something like this:

* The error from the stacktrace was  `TypeError: unsupported operand type(s) for +: 'int' and 'str'`.
* The line that triggered this error was this one: `c = a + b`
* Either of the first two lines is the problem since that's where these variables were created.
* The problem is that the code tried to add a string to an integer, which is not possible. 
* I'd fix this by having `a = "5"` so that I could concatenate the two variables together as a string.

And then you would fix the error in the code as you describe in your document.

### What to submit in your .zip file.
1. The document with the description of each bug, as described above. 
2. Your version of `ps7-buggy.py` with all five bug fixes.

---

## Part 2: Using the debugger


