# Week 1 Pre Homework
## Assignment
1. Create a git repository called Week1PHW and put it on github
2. Make two commits.  
    a. The first commit's message should be: ```"First commit."``` In that commit there should be only 1 file: HelloWorld.txt. The contents is one line that says: ```"Hello World!"```  
    b. The second commit's message should be: ```"Second commit."``` This commit should hold 2 files: ```HelloWorld.txt``` - change the contents of this file to be: ```"Hello World, I love CodeBase!"```. The second file should be named ```MentoredProject.txt``` and its contents should be one line that says: ```"The Mentored Project is the best."```
3. DM me a link to the Github repo. Here is an example of what the final repo should look like: <https://github.com/bdeleonardis1/Week1PHW/>
4. **Deliverable:** Make sure you understand what the following commands do: ```git clone```, ```git add```, ```git commit```, ```git push``` and ```git status```. If any of these are confusing to you consult the resources section at the end of the document.

##### If you feel reasonably comfortable with git, I recommend that you try to complete the assignment on your own (it will probably go faster). If you've never used git before I recommend going through guide below, but feel free to try to google around to figure it out.

## Git Guide
### Introduction
Git is a version control system. Version control systems keep track of changes that you made to files so that you can restore old versions of the codebase (like the one that actually works!). Git also allows you to collaborate with other people and store multiple versions of the same codebase at once.

### Install Git (skip if you've installed already - most of you probably have)
* Mac Users - Open a terminal and run: ```brew install git```
* Linux Users - Open a terminal and run: ```sudo apt-get install git```
* Windows Users - Visit <https://git-scm.com/download/> and click on Windows. Open up the installer and click through (defaults should be fine). **Note that if you've installed git bash for 61A, you've already installed git and you do not have to do this**

### Create a Github Repository
1. Visit <https://github.com> and create an account if you haven't already.
2. Click the greenbox that says *New Repository* (on the right side), then give the repo a name, and finally click *Create Repository*

### Clone the repository to your machine
1. Open up a terminal (for Windows users terminal = git bash)
2. Navigate (by using the cd command) to the parent folder where you want to store this repo (you should probably create a CodeBase folder)
3. Run git clone <insert the url under quick setup after you created the repository>  
    a. The url should look something like *github.com/<your_username>/<your_repository name>.git*


### Your first commit
1. cd into the repository you just cloned (it will be in a folder called <repository name>)
2. Create the ```HelloWorld.txt``` file  
    a. To do this quickly just type: ```touch HelloWorld.txt``` in your terminal
3. Write ```Hello World!``` in this file  
    a. To do this quicky type ```echo "Hello World!" > HelloWorld.txt```
4. Run ```git add .``` - This tells git to start tracking all the files in your current folder  
    a. Alternatively, you could run ```git add <filename>``` to only add the file, or ```git add -A``` to add all of the files in the repo
5. Run ```git commit -m "First commit"``` - This tells git to save your current CodeBase (in the form of a commit). ```-m``` tells git that what comes next is the message and the message goes in quotes
6. Run ```git push origin master``` - This tells git to upload all of your local commits (your saved versions of the codebase) to the github repository, you can ignore the origin master part, we'll learn about what this does in lecture

### Your second commit
1. Change HelloWorld.txt to read ```Hello World, I love CodeBase!``` (it's probably easiest to just open a text editor to do this)
2. Create MentoredProject.txt and add the line ```The Mentored Project is the best.```
3. Run ```git add -A```
4. Run ```git status```. This tells you what files git is tracking and whether they have unsaved changes. Try to interpret the output and get a feel for what it does.
5. Run ```git commit -m "Second commit"```
6. Run ```git push```

### Confirm it worked on github
1. Vist the github repo you created earlier and confirm everything worked
2. DM me the url

## Resources
If you needed to go through the guide I highly recommend going through: <https://try.github.io/levels/1/challenges/1>. You can stop when it starts talking about branching. This tutorial will create the git repo in a new way and it will also go over remotes (something I skipped over).  
Here are some universally useful resources:

* <https://www.cloudways.com/blog/git-tutorial-for-beginners-version-control/> - some more in depth explanations for the basic commands
* <http://marklodato.github.io/visual-git-guide/index-en.html> - introduces diff, checkout, reset commands and has great pictures
* <https://wikileaks.org/ciav7p1/cms/page_1179773.html> (advanced) - only look at it after lecture on Sunday. I've referred to this page numerous times which is why I included it



