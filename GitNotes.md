# Everything You Wanted To Know About Git
![GitIcon](git-icon.png)

You won't find it on this page.

Look [here](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/#1) instead. 

But I will tell you a little about Git to show off some nifty Markdown I haven't used before.

You can do a ton of things with Git to facilitate distributed team software development. It is a DVCS - Distributed Version Control System. Boo yah! Thanks again Linus Torvalds. 

Here is a summerized list of commands to enable a sub-setted basic workflow. 

```
$ cd test 
$ git init
$ git add *.md
$ git add LICENSE
$ git commit -m “any message here”

// cloning a repo
$ git clone https://github.com/test 
// or
$ git clone https://github.com/test mydirectory

// most useful of all git commands 
$ git status

// add a file 
$ git add filename

// add files
$ git add *

// commit a change
$ git commit -m “made change x,y,z”

// or commit all changes
$ git commit -a

// push changes to master
$ git push origin master
```
