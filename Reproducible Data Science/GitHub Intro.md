# Introduction to GitHub

Throughout this course, we'll be using a platform called [GitHub](https://github.com/). GitHub is a popular code hosting platform. It has lots of features that make version control and collaboration easier. Version control refers to the techniques for managing changes to software and code, and easily going back and forth between older and new versions of a code base. Getting familiar with GitHub and all of its tools can take some time, but the benefits for open science and streamlined collaboration are worth it.

At some point in your career, you have probably found yourself in a situation like this:

![Final.doc](https://github.com/Akesari12/Computational-Social-Science-Labs/blob/master/images/phd_comics_final_doc.png?raw=true)

GitHub is a useful tool because it removes a lot of the obstacles that we usually face when we are collaborating with others. Instead of saving multiple versions of the same document, GitHub lets us iterate on the same document while recording how it has changed over time. Rather than sending collaborators messily named documents, everyone can work from the same GitHub repository. GitHub also has tools for resolving editing conflicts between collaborators and creating a clear workflow.

# Getting Started

First, let's get started by making GitHub accounts. Navigate to GitHub's [homepage](https://github.com). Navigate to "Sign Up" in the top right hand side of the page. I recommend you create an account using your berkeley.edu account.

![Sign Up](https://github.com/dlab-berkeley/Computational-Social-Science-Training-Program/blob/master/images/github%20sign%20up.png)

After today's lab, I recommend you head over to GitHub Education and follow the instructions for activating your [free student developer pack](https://education.github.com/pack/offers). The student developer pack is free for as long as you are a student, and offers several benefits. The most important one of these will be GitHub Pro which gives you access to more collaboration tools and the ability to make unlimited private repositories. You might also consider exploring some of the other benefits like access to cloud services like Amazon Web Services or Microsoft Azure. 

# Navigating GitHub

## Interacting with Other Repos

GitHub is built on top of [git](https://en.wikipedia.org/wiki/Git), which is a Linux-based version-control system. Git is used by software engineers and data scientists to track changes in code and other files, work together, and support distributed workflows. GitHub builds on top of the core toolkit by providing a suite of tools and graphical interfaces that streamline collaboration and code organization. Let's take a look at some of the features on the webpage. The first thing we will look at is how to interact with other users' repositories. Follow along by navigating to the GitHub repo for the [Computational Social Science](https://github.com/dlab-berkeley/Computational-Social-Science-Training-Program) course. 

![Interact With Repos](https://github.com/dlab-berkeley/Computational-Social-Science-Training-Program/blob/master/images/repo%20interaction.png)

There are three basic ways you can interact with someone else's repo:

- **Watch**: Notify you when there are changes or conversations in the repo.
- **Star**: Add this repo to a list of repos that appear in your feed. Think of this as "favoriting" a repo.
- **Fork**: Make a copy of this repository in your own account. This is useful if you are not directly involved with a project but want to build on top of someone else's code.

GitHub can be a great resource because it provides access to the world's largest collection of source code, and it hosts many open source projects. Depending on your field, there may already be lots of repositories available that are worth exploring. Try to do the following steps:

1. Find the search bar in the top left.
2. Search for repositories based on some key words that are common for your field. For example, try searching "public health" or "economics."
3. Star and/or fork a repository that you find.

You can also follow specific users to see all of the repositories associated with them. This is a great way to see what others are working on and keep up to date with new developments. For example, try navigating to [Aniket's page](https://github.com/akesari12/) page and following it. 

## Create Your Own Repo

Next, let's look at how to make your own repos. Over time, you will create new repos to host code for your projects and collaborations. Doing so will help others reproduce your code, and serve as a useful way to showcase your work to employers and other social scientists. From the GitHub homepage, look for the "New" button near the top left.

![New Repo](https://github.com/dlab-berkeley/Computational-Social-Science-Training-Program/blob/master/images/github%20new%20repo.png)

Once you do this, click the green button, then name your new repository "My First Repository" or whatever else you like. Make sure you click the box to initialize it with a README.

![Initialize New Repo](https://github.com/dlab-berkeley/Computational-Social-Science-Training-Program/blob/master/images/github%20create%20repo.png) 

# Git from Command Line

## Configure credentials

Now we will see how to use some of git's core functions to work with repos and use version control. First, make sure to configure your global options for GitHub so that you don't have to login every time you want to do something. Open a bash terminal and do the following (substitute your GitHub handle and username):

```
git config --global user.name "Your Username"
git config --global user.email "your.email@berkeley.edu"
```

Then to make sure you only need to type in your password once, run the following:

```
git config --global credential.helper cache
```

