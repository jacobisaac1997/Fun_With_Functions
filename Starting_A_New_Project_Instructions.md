# Read Me File to start a program(This is what shows up in bold):
	Example: Fun_With_Functions_Project

1. Start Eclipse
2. Change the Workspace to our flash drive
	: File>Switch Workspace
3. Start a new project: Fun_With_Functions_Project
	: File> New> Java Project
		: Use Default runtime environment
			then click finish
4. Add a new class with our new
	project selected: Fun_With_Functions
	: File> New> Class
		: New it, select public static void main
			option and finish.
Now begin Git on the local machine and Git Hub on the remote.
1. Open Command Prompt
	:Start> search cmd> Strike enter
2. Go to your project folder
	:E to change to the flash drive
	:dir to list the directory
	:E:\>cd Eclipse G to change to the correct workspace.
	:E:\Eclipse G>cd Fun_With_Functions_Project
	:E:\Eclipse G\Fun_With_Functions_Project
	You should be able to see the src and bin folders.

 Directory of E:\

09/09/2015  08:47 AM    <DIR>          Eclipse G
09/15/2015  12:15 PM    <DIR>          Eclipse G2
09/30/2015  09:50 AM            15,601 Github documentation.docx
               1 File(s)         15,601 bytes
               2 Dir(s)  15,823,994,880 bytes free
3. git init to begin a new local repository.
E:\Eclipse G\Fun_With_Functions_Project>git init
Initialized empty Git repository in E:/Eclipse G/Fun_With_Functions_Project/.git
/
4. git add. to add my files.
E:\Eclipse G\Fun_With_Functions_Project>git add .

5. git config our user name and email.
E:\Eclipse G\Fun_With_Functions_Project>git config user.name "Jacob Isaac"

E:\Eclipse G\Fun_With_Functions_Project>git config user.email "isaacj@student.sw
osu.edu"

6. Start a browser of choice
7. Go to Github "github.com"
8. Log into your personal account
9.Add a new repository
	: Name it, and make it public, but do not initilize your folder with a 
		read me file. That intilization makes my life annoying.
	:Press "Create Repository"
10. Follow the online instructions on how to
	…or push an existing repository from the command line

git remote add origin https://github.com/jacobisaac1997/Fun_With_Functions.git
git push -u origin master
So go back to the command prompt, and do the first line, after enter do the second.

//The first line does fine
E:\Eclipse G\Fun_With_Functions_Project>git remote add origin https://github.com
/jacobisaac1997/Fun_With_Functions.git

//The second line doesn't like it.
E:\Eclipse G\Fun_With_Functions_Project>git push -u origin master
error: src refspec master does not match any.
error: failed to push some refs to 'https://github.com/jacobisaac1997/Fun_With_F
unctions.git'
//Here the local did not complain
E:\Eclipse G\Fun_With_Functions_Project>git commit -m "first commit"
[master (root-commit) 90d502c] first commit
 4 files changed, 35 insertions(+)
 create mode 100644 .classpath
 create mode 100644 .project
 create mode 100644 bin/Fun_With_Functions.class
 create mode 100644 src/Fun_With_Functions.java

E:\Eclipse G\Fun_With_Functions_Project>git push
warning: push.default is unset; its implicit value has changed in
Git 2.0 from 'matching' to 'simple'. To squelch this message
and maintain the traditional behavior, use:

  git config --global push.default matching

To squelch this message and adopt the new behavior now, use:

  git config --global push.default simple

When push.default is set to 'matching', git will push local branches
to the remote branches that already exist with the same name.

Since Git 2.0, Git defaults to the more conservative 'simple'
behavior, which only pushes the current branch to the corresponding
remote branch that 'git pull' uses to update the current branch.

See 'git help config' and search for 'push.default' for further information.
(the 'simple' mode was introduced in Git 1.7.11. Use the similar mode
'current' instead of 'simple' if you sometimes use older versions of Git)

fatal: The current branch master has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin master

E:\Eclipse G\Fun_With_Functions_Project>

//Pushing the master branch to github successfully
E:\Eclipse G\Fun_With_Functions_Project>git push --set-upstream origin master
Username for 'https://github.com': jacobisaac1997
Password for 'https://jacobisaac1997@github.com':
Counting objects: 8, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 1.14 KiB | 0 bytes/s, done.
Total 8 (delta 0), reused 0 (delta 0)
To https://github.com/jacobisaac1997/Fun_With_Functions.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
