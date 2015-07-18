---
layout: post
title:  "Setting up a development library"
date:   2015-07-15 15:03:08
categories: javascript
---

# Writing JavaScript Outside of the Browsers Console

If you've been using Codecademy or another browser based learning tool, you  might be wondering where you can save your code and come back to it later, or how you would write and store this code if you weren't using the in browser editor. The answer is in a text editor. You would write and save your file using the .js extension. So if you want to build a program to track cats in your neighborhood, you would save it as cats.js. If you are adding your JavaScript to a static website, you would save it in the same folder and possibly name it scripts.js, or alertbox.js depending on what you were doing. A lot of engineers and developers call your text editor of choice + how you configure it + how you configure your terminal and any other personal touches your "development environment." There are a lot of different ways to configure this, and while people might have strong opinions on which text editor is better, it all comes down to personal preference.  This section will cover some of the options available and how you might set it up. 

# Cloud and Browser Based Services

If you do not want to download a text editor or are using multiple computers and machines and don't want to have to re-configure things often, using a browser based development environment might be for you. There are many different kinds available, some have awesome built in features or add on plugins, and some are simply text editors for playing with small bits of cade.

## JSFiddle

If you want to play around with small bits of code and see how it would run in the browser, you can use [JSFiddle](https://jsfiddle.net/). You can add HTML and CSS, too, so you can get an idea of what it would look like to a visitor of a webpage. You can save your work and send it to someone else or you can then put it into your actual code. This is useful if you want to extract a small bit of code from your project and play around with different variable or values to see what looks best or works best. It's not a complete online development environment, but it is a good place to practice and try new things. 

## Codepen

Like JSFiddle, [Codepen](http://codepen.io/) allows you to write your code in the browser. According to the website, "it is an HTML, CSS, and JavaScript code editor in your browser with instant previews of the code you see and write." It has a free plan, but also paid plans that allow you to collaborate on projects with other people. You can get inspiration, or learn cool tricks from other public projects. It's got a great community that takes its [Code of Conduct](http://blog.codepen.io/legal/code-conduct/) seriously so that everyone feels safe and welcome.

## Cloud9

[Cloud9](https://c9.io/) is an entirely cloud-based fully functional development environment. It has a built in Terminal, a debugger, language tools, split screens and tabs, themes, and can be set up like vim, emacs, or sublime text editor (we'll get to those in a moment!). If you're worried about a typo breaking your computer in the Terminal, or downloading yet another program to your desktop, give Cloud9 or another browser based development environment a try. They have a free plan you can use until you decide to either sign up for a larger monthly plan, or try a text editor and your own terminal. 

## Koding

[Koding](https://koding.com/) was one of the first to the cloud-based dev environment scene, and it is still free to use. Plus NASA uses it. It might not have all the themes and customizations of Cloud9, but it's got a core set of features for free that you can use.

# The Terminal 

The Terminal (Or PowerShell or cmd in Windows) is an operating system without all the buttons. What you usually use to navigate a computer is called a "graphical user interface" or GUI. The GUI is the buttons on your desktop, the visual installation wizards, and the folders you see in your desktop. Using the Terminal,  you can type commands in and install, edit, or create new documents. Using the Terminal can let you quickly navigate your computer completely by keyboard. It's usually pretty safe, too. A single typo won't completely destroy everything, and as long as you stay away from "sudo" unless you really need to, almost everything is reversible. 

## Basic Commands

If you are on Mac you can find the terminal by using command + spacebar to get the spotlight, then typing in Terminal. If you are on a Linux system, you can search for Terminal, it should come already installed. Once you've opened it, it should have you in your home directory.  

The first command you want to know is "ls" which is the command you use to list the files in the directory you are currently in.  Some files are hidden files, these are system files or otherwise important files that you do not want showing up in the GUI and accidentally deleting. You can see these by using "ls -a" for list all. The -a is called a flag. Most commands can take a variety of flags that modify the way in which they behave. 

Once you know which files or sub directories are in there, you can also create them. You want do use "mkdir (directory_name)" to make a new folder. If I wanted to make a folder for my cat pictures, I could type mkdir cat_photos into the command line. 

If you want to make a file, you use the "touch" command. So if I wanted to make a JavaScript file to write a program for cats, I could write in the command line "touch catscript.js"!

So how do you open that JavaScript file? You can set custom commands in your bash profile, or there should be some added when you install certain software. For example, if you use the Sublime text editor, you can type "subl catscript.js" and it will open Sublime with catscript.js. If you have a whole directory of files you want to open at once, you can use . which means "all". Typing "subl ." in the directory you want to open will open all of the folders and files in that directory. 

Sometimes you have to move around your computer though. You can find out where you currently are by typing pwd, which stands for present working directory. If you want to change, you type "cd Directory/I/Want/To/Move/To". You can type the first letter or two and then use the tab key to cycle through the directories and use the tab-complete. The ~ is automatically set as your home directory, so typing cd ~ will take you back to the root. 

The Terminal is pretty powerful, and there are a lot more helpful commands to know. For more in depth, I recommend [Learn Command Line The Hard Way](http://cli.learncodethehardway.org/book/).


## Bash Profile

## Getting some basic things installed

JS Runtime
npm
curl

# Git and GitHub

One powerful command line tool is 'git.' You know that school project or that work project where multiple people were involved? You had Project_draft_1 ... Project_draft_10 but then you also had Project_FINAL, and then you had Project_FINAL_2, and soon you had Project_FINAL_FINAL, but before long you also had Project_FINAL_FINAL_FOR_REAL and it became a nightmare from a hell dimension because Laura was working from Project_FINAL_FINAL and Juan was working from Project_FINAL_FINAL_FOR_REAL and merging those two together was gonna be difficult. 

This is what git is for. Git is version control software to help manage this problem. You have a 'master' branch, where all the code you really like goes. You can then create branches to work on code that isn't quite finished or ready yet. If you are working alone, you can create branches for new feature or things you want to try out. You can do this in groups, too. Or, you can each have your own branch to work on your own set of things. Once the code is to a point where you want to merge it into master, you can do a merge and it will either automatically merge it, or if there are conflicts, it will tell you which lines have conflicts, and let you decide which version you want to keep or discard. Everything you commit to the git repository is saved, so you can reset to an earlier part of the repository. It's kind of like track changes in Word. 

GitHub is a place to keep your projects on the web. You can 'push' your code up or 'pull' code down. A lot of teams use Github as a way of keeping all the code straight. You work on a branch, push it to Github, and then a team member can pull that branch down from Github. It also provides a way to graphically manage merges with it's pull request feature, and other graphical user interface niceties. You can create a wiki for your project with instructions on how to get set up, and use the issue tracker to discuss what you want to work on next or track bugs you are currently encountering. 

## Git CLI

If you would like to use the command line to manage your git, here are a set of basic commands to get you started. There are some GUI programs for managing git, for example, [GitX](http://gitx.frim.nl/) for OSX or [GitEye](http://www.collab.net/products/giteye) for Mac, Windows, and Linux. 

_git init_  

git init sets up the current directory as a git repository. If you create a folder to start your project in, you'll want to run this at the start. It will create a .file (dot file, or a file that is only visibile in the terminal) that will track your changes and commits and branches. 

_git clone {   }_

clone a repository to your local machine. Using the git clone sha address in GitHub will clone the repo, initialize it, and automatically set it as a remote. If there is a repo you want to collab on, you can clone the repo directly, or fork it in github the clone the repo that is in your profile.



_git push (origin/upstream) (staging/master/branch_name)_

Push code to a remote repository. 

_git pull (origin/upstream) (staging/master/branch_name)_


_git remote_
_git checkout_
_git add_
_git commit_
_git merge_

# Downloading a Text Editor

If you don't want to work in the browser, you can use the Terminal your computer already comes with and download a text editor of your choice. There are MANY text editors out there, and a constant source of developer friendly-debates is which one is best. The answer is: whichever one works best for you! This will have a short list of free or nearly-free text editors to try out. 

## Atom

[Atom](https://atom.io/) is a free text editor that was created by the engineers at GitHub, they say it is "hackable" since you can download the source code and add to it if you would like. Currently it is only available on Mac's, although Window's and Linux versions are said to be coming. 

## Sublime Text  


## VIM

## Emacs