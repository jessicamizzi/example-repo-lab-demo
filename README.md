# This is the readme file. It can be used to described what is in your repository!

The README file can be formatted in RST or Markdown. Because I have the file named README.md, it will be read as a Markdown file by GitHub. To use RST, save the file as README.rst. A markdown cheatsheet can be found here: [https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).

## Steps to putting existing repository on GitHub:

1. Go into directory (directory = folder in file system) and create a file. I’m using vi, which is a text editor at the command line, but you can also a program like TextEdit on a Mac or WordPad on a PC to make a .txt file. (Note - it’s better to save files as plain text, which defaults to a .txt format, rather than rich text, which defaults to .rtf, because rich text has hidden formatting characters that mess with encoding.) This is the folder where you would keep your scripts.

2. Type `git init`. This initializes a program called “git”, which is a version controlled system called git that tracks all the changes you make to your files. git is integrated with GitHub, which hosts these repositories online.

### Putting repo on GitHub 
Extra info is here: [https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/](https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/)

3. (Optional) See status of file. Type `git status`, and you will see the file in your repository as “untracked”.

4. Add files to tracking. Type `git add .` this will add all the files in your repository to the tracking. The `.` means everything in the current directory. You can also type `git add [file name]` to only track specific files, making sure to replace [file name] with the file you want to add.

5. Commit files. This is “committing” to push these changes up to github. If you have added a file you don’t want to push to github, you can still remove it. Type `git commit -m “first commit of this repo”`. The “first commit of this repo” is called a commit message, and can be used to identify what changed at each commit, so it’s a good idea to succinctly describe what you did in this commit. If you forget the `-m “message here”` part of the command, then a different text editor program called nano will open up for you to insert your commit message, but I find it more convenient to insert the message with this command.

6. Go to github.com and log in, then click the plus button in the upper right hand corner, or go to [github.com/new](github.com/new). I like to name the repo whatever I’ve named the directory. You can give a repo description now or later or never), I make them all public (private repos must be purchased, but if can verify you have an academic email, you can get some free private repos, I think 5?), I generally don’t initialize with a readme, but it doesn’t really matter at this stage unless you already have a file called `README.md` in your local repo because this will overwrite it.

7. Now, copy the following lines of code you are given when in your local repo:
```
git remote add origin https://github.com/jessicamizzi/example-repo-lab-demo.git
git push -u origin master
```

You might need to do some configuration of your username if that’s not set up yet.

8. Now you can push changes.

9. If you have made changes to the online repository, you need to pull them down before creating additional changes. Type `git pull` to do this.
