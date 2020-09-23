## [Diff and Patch Cheat Sheet](https://www.coursera.org/learn/introduction-git-github/supplement/cKIs3/diff-and-patch-cheat-sheet)

**diff**
diff is used to find differences between two files. On its own, it’s a bit hard to use; instead, use it with diff -u to find lines which differ in two files:

**diff -u**
diff -u is used to compare two files, line by line, and have the differing lines compared side-by-side in the same output. See below:

```
diff -u menu1.txt menu2.txt
```

**Patch**
Patch is useful for applying file differences. See the below example, which compares two files. The comparison is saved as a .diff file, which is then patched to the original file!

```
diff -u hello_world.txt hello_world_long.txt > hello_world.diff
patch hello_world.txt < hello_world.diff
```

There are some other interesting patch and diff commands such as patch -p1, diff -r !

Check them out in the following references:

http://man7.org/linux/man-pages/man1/diff.1.html
http://man7.org/linux/man-pages/man1/patch.1.html
