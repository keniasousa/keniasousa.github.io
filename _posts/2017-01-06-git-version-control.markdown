---
layout: post
title: "Git:  How to know if your directory is already under version control?"
date: 2017-01-06 16:27:20 +0200
categories: data analysis git
---

Say you have started working in a new project and there was no hand-over file from the previous developer. Before you start, you want to know if the a directory is under version control.

There are, of course, several options to find this out, depending on what you need, such as do it manually in command line or in your program in python, etc. For that, just Google it and you’ll find solutions, such as this one on <a href="http://stackoverflow.com/questions/2044574/determine-if-directory-is-under-git-control" onclick="javascript:pageTracker._trackPageview('/outbound/article/stackoverflow.com');" target="_blank">stackOverflow</a>.

Now, I just want to determine if my directory is under control.

<strong>First option:</strong> Go to the command line, move to your directory and type:

```
$ git status
```

<img src="/images/posts/git-status.png" class="git-status" alt="Git Status">

The result is shows that there are no changes, thus, nothing to commit.<br/>
Note that I used

```
$ git status -u no
```

From the <a href="https://git-scm.com/docs/git-status" onclick="javascript:pageTracker._trackPageview('/outbound/article/git-scm.com');" target="_blank">Git documentation</a>, you see that -u no is used to hide untracked files. I had tried before without it and it showed a long list of untracked files that did not allow me to see anything else. Since my goal here is just to see if it is under version control, that message is enough.

Just before, you see that I tried with another folder, which is not under version control, and the error message confirms that it is not a git repository.

<strong>Second option:</strong> Using SourceTree:

1) Open to SourceTree<br/>
2) Click on “Create/New”<br/>
3) Click on “Add Working Copy”

<img src="/images/posts/source-tree.png" class="source-tree" alt="Source Tree">

4) See on the list of “Unstaged files” that files are:<br/>
– Clean<br/>
– Modified<br/>
– Missing<br/>
– Not tracked<br/>
For the modified: On the right, you can see what was changed in the content.

On the top left: you can see how many files were:<br/>
– Added<br/>
– Modified<br/>
– Not tracked<br/>

<img src="/images/posts/source-tree-files.png" class="source-tree-files" alt="Source Tree Files">

5) When you click on the master branch, you see that a commit was done and see all the files that were committed at the bottom and their content on the right.

<img src="/images/posts/source-tree-branches.png" class="source-tree-branches" alt="Source Tree Branches">

Now that you are sure your directory is already under version control, you can drag and drop the files to the list of “Staged files” on top, which will be included in the next commit.

<img src="/images/posts/source-tree-staged-files.png" class="source-tree-staged-files" alt="Source Tree Staged Files">

For more references, check out the Coursera Course on Data Scientist Toolbox available on github (<a href="https://github.com/bcaffo/courses/blob/master/01_DataScientistToolbox/02_06_01_createNewRepo/index.md" onclick="javascript:pageTracker._trackPageview('/outbound/article/github.com');" target="_blank">create new repo</a>, <a href="https://github.com/bcaffo/courses/blob/master/01_DataScientistToolbox/02_06_02_forkRepo/index.md" onclick="javascript:pageTracker._trackPageview('/outbound/article/github.com');" target="_blank">fork and clone a repository</a>, <a href="https://github.com/bcaffo/courses/blob/master/01_DataScientistToolbox/02_07_02_gitWorkflow/index.md" onclick="javascript:pageTracker._trackPageview('/outbound/article/github.com');" target="_blank">git workflow</a>, <a href="https://github.com/bcaffo/courses/blob/master/01_DataScientistToolbox/02_07_01_basicGitCommands/index.md" onclick="javascript:pageTracker._trackPageview('/outbound/article/github.com');" target="_blank">basic Git Commands</a>) as well as this quick Git guide from the <a href="http://www.dataschool.io/git-quick-reference-for-beginners/" onclick="javascript:pageTracker._trackPageview('/outbound/article/www.dataschool.io');" target="_blank">Data School</a> and more on the <a href="http://datasciencespecialization.github.io/toolbox/" onclick="javascript:pageTracker._trackPageview('/outbound/article/datasciencespecialization.github.io');" target="_blank">data scientist’s toolbox site</a>.
