Git Workshop Instructions
=========================

##Usefulness
A Github account is almost a necessity when it comes to sharing code with a large audience, especially in the start up world. This is also great for getting jobs / internships and it allows you to work on tons of open source projects. Furthermore, if you want to start an open source project, there's no better place to start than with Github!

##What is Git?
Git is a free and open source version control system. In our opinion (and popular opinion) it is the best. Many companies require employees to know git.

##Usage!
Install with `sudo apt-get install git` (Linux) or `brew install git` (Mac) `????` (Windows)

Initialize a repository `git init` OR create it on Github and `git clone <repository_address>`. Add some files! `git add <filename>`. If you want to remove files? `git rm <filename>` Move files: `git mv <filename> <new_filename>`.

To check what changes you have made: `git status`

Side note: If you want to read the man pages for any command, for example add, use `man git-add` (hyphenate the word 'git' and the command).

How to commit your files! `git commit` But some useful flags: `git commit -m "Here's a commit message"` (`m` is the most important) `git commit -am "All modifications not staged for commit WILL BE COMMITTED"` (`a` can be dangerous)

What do I do with all the files that I don't want to commit? (For example `.DS_Store`) Add them to your git ignore file, that is a plain text file at the top level of your directory called `.gitignore`! This project has one too.

Now time to send / receive files from a remote repository: `git push <host> <branch>` or `git pull <host> <branch>` [or first `git fetch -a` then `git merge <branch>` will merge `<branch>` into the current branch]

`tig` is a nice way to view your history.

##Using Branches
Add a remote host: `git remote add <name> <full_host_path>`
Change branch: `git checkout <branch>`

(See Also: [[http://gitref.org/]])